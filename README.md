# XO Game - Online Multiplayer Tic-Tac-Toe

A real-time multiplayer Tic-Tac-Toe game built with Next.js and Convex backend.

## Features

- Create and join game rooms with unique room codes
- Real-time gameplay with automatic turn handling
- See who's online in your game room
- Waiting room with list of available games
- Responsive design that works on mobile and desktop

## Convex Configuration

This project uses Convex as its backend with the following configuration:

```
convex key
dev:adorable-spider-894|eyJ2MiI6ImU4MTRmYTlhODUxOTQzNjM4YWFiMGFjODkwZDc5YmY2In0= 
dev link 
@https://adorable-spider-894.convex.cloud  
HTTP Actions URL
@https://adorable-spider-894.convex.site 
```

## Getting Started

### Prerequisites

- Node.js 14+ and npm/yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd xo-game
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Create a `.env.local` file with your Convex URL:
   ```
   NEXT_PUBLIC_CONVEX_URL=https://adorable-spider-894.convex.cloud
   ```

4. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to see the game.

## How to Play

1. Enter your name on the home page.
2. Either:
   - Create a new game room by clicking "Create Game"
   - Join an existing game by entering a room code and clicking "Join"
   - Join one of the available rooms in the list below

3. Share your room code with a friend so they can join.
4. Players take turns placing X's and O's on the board.
5. The first player to get three in a row wins!

## Deployment

This project can be deployed to any static hosting service that supports Next.js, such as Vercel:

```bash
npm run build
# or
yarn build
```

## Technology Stack

- **Frontend**: Next.js, React
- **Backend**: Convex (serverless backend with real-time sync)
- **State Management**: React hooks with Convex queries and mutations
- **Styling**: CSS with custom variables

## Project Structure

```
/
├── components/       # Reusable React components
├── convex/           # Convex backend functions and schema
├── hooks/            # Custom React hooks
├── pages/            # Next.js pages
├── styles/           # Global CSS styles
└── public/           # Static assets
```

## License

MIT 