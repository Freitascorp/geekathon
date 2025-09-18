# GreenPath Project Brief

**Project:** GreenPath - AI-Powered Sustainable Mobility Rewards Platform  
**Objective:** Create a complete, functional MVP for a geekathon competition that incentivizes sustainable transportation choices through token rewards. The application must be fully operational within 48 hours.

---

## Core Requirements

**Multi-Component System**
- React Native mobile app
- Node.js/Express backend API
- Ethereum/Polygon smart contract
- Google Maps API
- Real-time location tracking

**Key User Journey**
1. User enters start/destination.  
2. System calculates routes with carbon impact scores.  
3. User selects sustainable route.  
4. App launches navigation app.  
5. Background tracking validates route completion.  
6. Automated token rewards.

**Technical Stack**
- **Frontend:** React Native with `react-native-maps`, `react-native-geolocation-service`
- **Backend:** Node.js, Express, Google Maps APIs
- **Blockchain:** Solidity smart contracts on Polygon Mumbai testnet
- **Database:** Simple JSON/SQLite for demo purposes

---

## Specific Implementation Tasks

### Backend
- Create endpoints for route calculation and token minting
- Implement carbon algorithm
- Integrate Google Maps
- Set up ethers.js

### Frontend
- Create navigation stack
- Implement address input
- Add map visualization
- Build deep linking
- Implement background tracking
- Create wallet display

### Blockchain
- Deploy ERC-20 contract
- Implement minting function

---

## Deliverables
- Fully functional React Native app  
- Live backend API  
- Deployed smart contract  
- Complete user flow  
- Demo data  

---

## Success Criteria
- User can plan a route  
- App launches navigation  
- System tracks and validates trips  
- Tokens are minted automatically
