# Connectify: Social App Frontend

A React frontend exploring social interactions and **real-time GraphQL**. The application combines GraphQL queries, mutations, and subscriptions with client-side state and routing.

## Features represented in the frontend

- User registration and authentication flows
- Profiles, users, and feeds
- Friend requests and friend-list updates
- Messaging-related events and notifications
- Real-time updates through GraphQL subscriptions

## Technology

React 18 · Apollo Client · GraphQL · graphql-ws · Redux Toolkit · React Router · Material UI

## How it works

- Apollo Client handles GraphQL operations and caching.
- HTTP requests and WebSocket subscriptions use separate links.
- Redux manages frontend application state.
- React Router manages client-side navigation.

## Run locally

```bash
git clone https://github.com/Abi0l9/Connectify-frontend.git
cd Connectify-frontend
npm install
npm start
```

The frontend runs at `http://localhost:3000` by default.

**Backend requirement:** The current Apollo configuration expects a compatible GraphQL service at `http://localhost:4000` and subscriptions at `ws://localhost:4000`. The backend is **not included in this frontend repository**, so interactive functionality requires that service to be running.

## Where to look

- `src/index.js`: Apollo HTTP/WebSocket link setup
- `src/App.js`: top-level queries, subscriptions, and client-side interactions
- `src/Queries/`: GraphQL operations
- `src/reducers/`: Redux state management

## Scope

This is a frontend code sample. The repository showcases React application structure and GraphQL integration; it does not claim to provide a standalone hosted social network.
