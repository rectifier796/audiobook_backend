# RESTful API Using Node, Express, Mongoose

The project builds RESTful APIs using Node.js, Express and Mongoose, ...

## Manual Installation

Clone the repo:

```bash
git clone https://github.com/libeyondea/backend-node-express.git
cd audiobook_backend
```

Install the dependencies:

```bash
npm install
```

## Table of Contents

- [Commands](#commands)
- [Environment Variables](#environment-variables)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)

## Commands

Running in development:

```bash
npm start
```

## Environment Variables

Create and modify `.env` file.

```bash
# Port
PORT = # default 5001

# URL of the Mongo DB
MONGO_URL = mongodb://127.0.0.1:27017/database_name

## Project Structure

```
config\         # Database configuration
controllers\    # Controllers
middlewares\    # Custom express middlewares
models\         # Mongoose models
routes\         # Routes
index.js        # App entry point
```

## Project Structure

```
public\             # Public folder
 |--index.html      # Static html
src\
 |--config\         # Environment variables and configuration
 |--controllers\    # Controllers
 |--middlewares\    # Custom express middlewares
 |--models\         # Mongoose models
 |--routes\         # Routes
 |--services\       # Business logic
 |--utils\          # Utility classes and functions
 |--validations\    # Request data validation schemas
 |--index.js        # App entry point
```

### API Endpoints

List of available routes:

**Routes**:\
`POST api/audio-book/create` - Create Audio Book\
`POST api/review/create` - Create Review\
`GET api/audio-book/get-details/slug/:slug` - Get Audio Book Details\
`GET api/audio-book/get-details/page/:pageId` - Get All Audio Book based on different search filters\
`GET api/audio-book/get-author` - Get List of all authors\
`GET api/audio-book/get-genre` - Get List of all genre\
`GET api/review/get-review/:audioBookId/:pageId` - Get all review by audio book id\
