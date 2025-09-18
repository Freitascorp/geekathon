# Product Requirements Document (PRD)

**Project Name:** GreenPath - AI-Powered Sustainable Mobility Rewards Platform  
**Version:** 1.0  
**Authors:** John, BMad Product Manager  
**Status:** Complete  

---

## 1. Introduction
This document outlines the requirements for the GreenPath MVP, an AI-powered platform for a geekathon competition.  
The primary goal is to incentivize sustainable transportation by rewarding users with digital tokens for eco-friendly travel choices.

---

## 2. Vision & Goals

**Vision:** Build a fully operational, multi-component MVP that proves the feasibility of an AI-powered system rewarding users for sustainable mobility choices.  

**Goals**
- **Operational MVP:** Deliver a functional React Native app, Node.js backend, and deployed smart contract.  
- **Seamless User Journey:** Ensure a complete user flow from route planning to token redemption.  
- **Competition Success:** Create a compelling, presentation-ready demo.  

---

## 3. Scope & Key Features

**In-Scope (Must-Haves):**
- Entire user journey: from route selection to automated token rewards.  
- **Frontend:** Navigation, maps, address input, deep linking, wallet display.  
- **Backend:** Route calculation API, token minting API, Google Maps integration, ethers.js.  
- **Blockchain:** ERC-20 smart contract with minting function.  

**Out-of-Scope (Future Considerations):**
- User authentication  
- Advanced tokenomics  
- Social features  
- In-app navigation  

---

## 4. Technical Requirements

**Frontend:** React Native, `react-native-maps`, `react-native-geolocation-service`  
**Backend:** Node.js, Express, ethers.js  
**Blockchain:** Solidity on Polygon Mumbai Testnet  
**APIs:** Google Maps Directions API
