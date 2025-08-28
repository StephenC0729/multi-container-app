# Multi-Container Todo App

A simple, containerized todo application built with Node.js, Express, MongoDB, and Docker Compose. Perfect for learning Docker multi-container applications and modern web development.

## Features

- ✅ Create, view, and delete todos
- 🐳 Fully containerized with Docker Compose
- 🔄 Hot reload development environment
- 📱 Responsive Bootstrap UI
- ⏰ Todo timestamps with moment.js
- 🗄️ MongoDB persistence

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Frontend**: EJS templating, Bootstrap 4
- **Development**: Nodemon, LiveReload
- **Containerization**: Docker, Docker Compose

## Quick Start

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd multi-container-app
   ```

2. **Start the application**
   ```bash
   docker compose up -d
   ```

3. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

4. **Stop the application**
   ```bash
   docker compose down
   ```

## Development

For development with hot reload:

```bash
docker compose up
```

The app will automatically reload when you make changes to the code.

## Project Structure

```
├── app/
│   ├── config/         # Database configuration
│   ├── models/         # Mongoose models
│   ├── routes/         # Express routes
│   ├── views/          # EJS templates
│   ├── server.js       # Main server file
│   ├── package.json    # Node dependencies
│   └── Dockerfile      # App container config
├── compose.yaml        # Docker Compose configuration
└── README.md
```

## Services

- **todo-app**: Node.js application (port 3000)
- **todo-database**: MongoDB database (port 27017)

## License

ISC