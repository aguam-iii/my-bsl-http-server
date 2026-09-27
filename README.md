# my-bsl-http-server
A lightweight, low-level HTTP web server constructed using the **Bonezegei Scripting Language (BSL)** and the BSL Socket Library (`lib/socket.bzg`).

## Project Overview

This project demonstrates how web servers interact at the socket layer. It manually handles incoming HTTP GET requests, parses requested endpoints (`/`, `/about`, or unknown paths), builds raw HTTP headers with custom HTML bodies, and returns appropriate status codes (`200 OK` or `404 Not Found`).

---

## Prerequisites & Installation Guide

### 1. VS Code Extension & BSL Interpreter
1. Open VS Code and go to the **Extensions tab** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Search for **Bonezegei** and install the **Bonezegei Scripting Language Formatter** extension.
3. Follow the extension guide to install the BSL Interpreter:
   - **Windows / Linux:** Follow native setup instructions in the extension.
   - **macOS / Android:** Use **GitHub Codespaces** with Linux instructions.

### 2. Install Socket Library
Run the following command in your terminal:
```bash
bzg install socket

### 3. Route Specifications

- **Landing Page (`/`)**: Responds with `HTTP 200 OK` and a welcome page.
  - URL: `http://localhost:8080/`
- **About Page (`/about`)**: Responds with `HTTP 200 OK` and project information.
  - URL: `http://localhost:8080/about`
- **404 Page (`/*`)**: Responds with `HTTP 404 Not Found` for unmapped routes.
  - URL: `http://localhost:8080/anything`

### 4. Screenshots Section

Screenshots are in the "Documentation" folder.
