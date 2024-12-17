# Online Blackjack

A **free-to-play, multiplayer blackjack game** designed for fun, accessibility, and an engaging online experience for players of all ages. Enjoy blackjack without the gambling aspects, play casually with friends, and customize your experience.

## Demo

[Link to Demo (YouTube)](https://youtu.be/cswk6KqHbqI)

---

## **Features**

- **Player Accounts**

  - Create accounts with a unique username and password.
  - Guest mode for quick and easy play (no account needed).
  - Manage profiles with stats and settings.
  - Win/loss stats displayed in-game and on profiles.
  - Customizable profile pictures based on user's skill.

- **Gameplay Mechanics**

  - Multiplayer lobbies with customizable rules.
  - Hosts can adjust:
    - Minimum/maximum bets.
    - Player count.
    - Turn timer limits.
    - Starting cash for each player.

- **Dynamic Game Interface**

  - Display player names and active turns.
  - Real-time updates for game progress.
  - In-game chat box for lobby communication.

## **User Roles**

### **Player**

- **Role**: Play and enjoy blackjack.
- **Tasks**:
  - Create/manage accounts or play as a guest.
  - View personal stats.
  - Join game lobbies and compete against others.

### **Host**

- **Role**: Manage game lobbies and player experience.
- **Tasks**:
  - Create lobbies with customizable game rules.
  - Manage player lists and remove disruptive players.

### **Administrator**

- **Role**: Maintain and improve the game.
- **Tasks**:
  - Monitor lobbies.
  - Resolve user issues.

## **Tech Stack**

### **Frontend**

- **React**: Dynamic and responsive user interface.
- **Tailwind CSS**: Efficient and clean styling for a visually appealing UI.

### **Backend**

- **Node.js & Express.js**: Backend server and API management.
- **MySQL**: Relational database for managing player data, stats, and lobbies.
- **WebSockets**: Real-time communication for seamless multiplayer gameplay.

### **Deployment**

- **Docker**: Containerized runtime environment ensuring compatibility and scalability.

## **Environment Variables**

You will notice the `.env` file is included within the database files. This is because the database runs locally, so security is not a concern.

In the backend, add the following to a `.env` file:

```
DB_HOST=<your-db-host>
MYSQL_ROOT_PASSWORD=<your-root-password>
MYSQL_DATABASE=<your-database-name>
JWT_SECRET=<your-jwt-secret>
```

## **Run Locally**

The project is Dockerized.

```bash
  docker-compose down && docker-compose up --build
```

To connect to the database:

```bash
  docker exec -it finalproject-database-1 mysql -u root -p
```

The password is found in the database `.env`.

## **Contributors**

- Matteo Cusanelli
- Jasmit Saroya
- Manjot Singh
- Brandon Smith
