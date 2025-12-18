# todo-db-mcp-toolbox-db

The purpose of this repo is to play with MCP toolbox for Databases, and how to use/consume MCP server through MCP client.

## Overview

This repository provides a setup for experimenting with the Model Context Protocol (MCP) toolbox specifically for database interactions. It includes:

- A PostgreSQL database initialized with a sample "todos" table containing 101 rows of fake data.
- An MCP server (toolbox) that exposes database tools for querying and manipulating the data.
- Docker Compose configuration to easily spin up the database and MCP server.
- A Dockerfile for building the MCP server image locally.

## Features

- **Database Setup**: PostgreSQL database with a pre-populated "todos" table (id as text, completed as boolean, order as integer, title as text).
- **MCP Server**: Toolbox MCP server that provides tools for database operations.
- **Docker Integration**: Easy deployment using Docker Compose.
- **Sample Data**: 101 todo items with random data for testing and demonstration.

## Setup

1. Ensure Docker and Docker Compose are installed.

2. Clone the repository and navigate to the directory.

3. Start the services:
   ```sh
   docker compose build
   docker compose up -d
   ```

   This will start the PostgreSQL database and the MCP toolbox server.

## Usage

Once the services are running:

- The database is accessible on the default PostgreSQL port (5432).
- The MCP server runs on port 5000.
- Use an MCP client to connect to the server at `http://localhost:5000/mcp` and access the database tools.

## Demo

<!-- Add GIF files here to demonstrate the MCP client interacting with the database tools -->
