# NodeJS - Docker - Sentry

A Node.js application with Docker containerization and Sentry error monitoring integration.

## Overview

This project demonstrates how to containerize a Node.js application using Docker and integrate Sentry for error monitoring and performance tracking.

## Technologies Used

- **Node.js** - JavaScript runtime for server-side development
- **Docker** - Containerization platform for consistent deployment
- **Sentry** - Error monitoring and performance tracking platform

## Project Structure

```
docker-node-sentry/
├── Dockerfile          # Docker container configuration
├── server.js           # Main Node.js server file
├── instrument.js       # Sentry instrumentation
├── package.json        # Node.js dependencies and scripts
├── pages/             # HTML pages
│   ├── exists.html
│   └── feedback.html
├── public/            # Static assets
│   └── styles.css
└── README.md          # This file
```

## Prerequisites

- Docker installed on your system
- Node.js (for local development)

## Quick Start

### Using Docker

1. Build the Docker image:
   ```bash
   docker build -t <image-name> .
   ```

2. Run the container:
   ```bash
   docker run -p 5000:5000 --name <container-name> --rm -d <image-name> 
   ```

3. Access the application at `http://localhost:5000`

### Using The Image from Docker Hub (login not required)

1. Pull image
   ```bash
   docker pull ahmedsallah0/feedback-node:1.0.0
   ```
2. Run Image in Container
   ```bash
   docker run -p 5000:5000 --name <container-name> --rm -d <image-name> 
   ```
   
## Sentry Integration (for fun)

## Features

- Containerized Node.js application
- Sentry error monitoring
