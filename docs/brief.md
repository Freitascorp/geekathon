1. Project Brief
Project: GreenPath - AI-Powered Sustainable Mobility Rewards Platform
Objective: Create a complete, functional MVP for a geekathon competition that incentivizes sustainable transportation choices through token rewards. The application must be fully operational within 48 hours.
Core Requirements:

Multi-Component System: React Native mobile app, Node.js/Express backend API, Ethereum/Polygon smart contract, Google Maps API, Real-time location tracking.

Key User Journey: User enters start/destination, system calculates routes with carbon impact scores, user selects sustainable route, app launches navigation app, background tracking validates route completion, automated token rewards.

Technical Stack:

Frontend: React Native with react-native-maps, react-native-geolocation-service.

Backend: Node.js, Express, Google Maps APIs.

Blockchain: Solidity smart contracts on Polygon Mumbai testnet.

Database: Simple JSON/SQLite for demo purposes.

Specific Implementation Tasks:

Backend: Create endpoints for route calculation and token minting, implement carbon algorithm, integrate Google Maps, set up ethers.js.

Frontend: Create navigation stack, implement address input, add map visualization, build deep linking, implement background tracking, create wallet display.

Blockchain: Deploy ERC-20 contract, implement minting function.

Deliverables: Fully functional React Native app, live backend API, deployed smart contract, complete user flow, demo data.

Success Criteria: User can plan a route, app launches navigation, system tracks and validates trips, tokens are minted automatically.
