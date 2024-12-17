# Online Blackjack

A **free-to-play, multiplayer blackjack game** designed for fun, accessibility, and an engaging online experience for players of all ages. Enjoy blackjack without the gambling aspects, play casually with friends, and customize your experience.

## Demo

[Link to Demo (YouTube)](https://youtu.be/cswk6KqHbqI)


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

<div class="flex items-center gap-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/react.svg" alt="React" width="18" height="18">
  <strong>React</strong>: Dynamic and responsive user interface.
</div>

<div class="flex items-center gap-2 mt-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/tailwindcss.svg" alt="Tailwind CSS" width="18" height="18">
  <strong>Tailwind CSS</strong>: Efficient and clean styling for a visually appealing UI.
</div>

### **Backend**

<div class="flex items-center gap-2 mt-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/nodedotjs.svg" alt="Node.js" width="18" height="18">
  <strong>Node.js & Express.js</strong>: Backend server and API management.
</div>

<div class="flex items-center gap-2 mt-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/mysql.svg" alt="MySQL" width="18" height="18">
  <strong>MySQL</strong>: Relational database for managing player data, stats, and lobbies.
</div>

<div class="flex items-center gap-2 mt-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/socketdotio.svg" alt="WebSockets" width="18" height="18">
  <strong>WebSockets</strong>: Real-time communication for seamless multiplayer gameplay.
</div>

### **Deployment**

<div class="flex items-center gap-2 mt-2">
  <img src="https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/docker.svg" alt="Docker" width="18" height="18">
  <strong>Docker</strong>: Containerized runtime environment ensuring compatibility and scalability.
</div>

## **Environment Variables**
> [!IMPORTANT]
> `.env` files are included in the database setup for simplicity, as this project runs locally.

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
