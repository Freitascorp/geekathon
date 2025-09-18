# System Architecture Document (AWS-First)

**Project:** GreenPath - AI-Powered Sustainable Mobility Rewards Platform  
**Version:** 1.1 (AWS-First)  
**Authors:** Winston, BMad Architect  
**Status:** Draft  

---

## 1. High-Level System Overview
The GreenPath platform will leverage a **serverless, event-driven architecture on AWS**.  

**Core Components**
- **Frontend (React Native):** Communicates with AWS API Gateway.  
- **Backend (AWS Lambda & API Gateway):** Contains route calculation and token minting logic.  
- **Data Storage (DynamoDB):** Stores user trip and reward data.  
- **Blockchain (Polygon/Smart Contract):** Handles token minting via Lambda.  

---

## 2. Data Flow & Interactions

1. The Frontend sends a request to an AWS API Gateway endpoint.  
2. API Gateway triggers a corresponding AWS Lambda function.  
3. The Lambda function executes business logic (e.g., Google Maps API call, carbon score, token minting).  
4. Data is read/written from DynamoDB.  
5. Lambda returns the response through API Gateway to the Frontend.  
6. For token minting, Lambda interacts with the Polygon blockchain.  

---

## 3. Component Breakdown & Technology Stack

### 3.1 Frontend: React Native Mobile App
- **Purpose:** User interaction layer.  
- **Changes:** API calls redirected to AWS API Gateway.  

---

### 3.2 Backend: AWS Serverless Components
- **AWS API Gateway:** Exposes REST endpoints mapped to Lambda functions.  
  - `POST /routes/calculate`  
  - `POST /rewards/mint`  

- **AWS Lambda:** Node.js functions following single responsibility principle.  
  - **calculateRoutesLambda:** Calls Google Maps API, executes carbon score algorithm.  
  - **mintTokensLambda:** Validates trips and securely calls smart contract `mint()` via ethers.js.  

- **Amazon DynamoDB:** Serverless NoSQL database for trip/reward records.  
- **AWS IAM:** Controls permissions (Lambda ↔ DynamoDB ↔ Blockchain).  

---

### 3.3 Blockchain: Solidity Smart Contract
- **Purpose:** Immutable token ledger.  
- **Changes:** Minting is invoked by `mintTokensLambda`.  
- **Smart Contract:** Remains unchanged.
