# Chappie - AI Model Frontend

This project implements Open WebUI as a frontend for AI/LLM models, made accessible through Cloudflare Tunnels.

## Overview

The project consists of two main components:
1. **Open WebUI**: Frontend interface for AI/LLM models
2. **Cloudflared**: Cloudflare tunnel service for secure internet access

## Architecture

- Host: Debian 12.9
- Internal Network: 192.168.1.0/24
- Open WebUI Address: 192.168.1.200
- Domain: chappie.jp8080.com

## Prerequisites

- Docker
- Docker Compose
- Git
- Cloudflare account with domain setup

## Project Structure

```
.
├── README.md
├── .env.example              # Example environment variables
├── .gitignore               # Git ignore file
├── docker/                  # Docker related files
│   ├── openwebui/          # Open WebUI configuration
│   └── cloudflared/        # Cloudflare tunnel configuration
├── docker-compose.yml      # Main compose file
└── docs/                   # Additional documentation
```

## Setup Instructions

1. Clone the repository
```bash
git clone [repository-url]
cd chappie
```

2. Copy and configure environment variables
```bash
cp .env.example .env
# Edit .env with your configuration
```

3. Start the services
```bash
docker compose up -d
```

## Development Workflow

1. Pull latest changes
2. Create feature branch
3. Make changes
4. Test locally
5. Push changes
6. Create PR

## Security Considerations

- All sensitive information is stored in .env file
- Cloudflare Tunnel provides secure access
- Internal services are not directly exposed to the internet

## License

[Your chosen license]
