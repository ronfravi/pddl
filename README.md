# PDDL Planning Environment

This project uses the `aiplanning/planutils` Docker image to provide a complete environment for PDDL planning, with full VSCode integration.

## Getting Started with VSCode

1. Make sure you have the following VSCode extensions installed:
   - Remote - Containers
   - PDDL
   - Python
   - Docker

2. Open this project in VSCode

3. When prompted, click "Reopen in Container" or:
   - Press `F1` or `Cmd/Ctrl + Shift + P`
   - Type "Remote-Containers: Reopen in Container"
   - Press Enter

VSCode will automatically:
- Build and start the container
- Install the necessary extensions
- Configure the development environment
- Open a new window connected to the container

## Available Tools

The planutils image comes with several planning tools pre-installed, including:
- FF (Fast Forward)
- LAMA
- LAMA-first
- Mercury
- Probe
- YAHSP
- And many more...

To see all available planners, run:
```bash
planutils --help
```

## Manual Container Access (Alternative)

If you prefer to use the container without VSCode:

1. Start the container:
```bash
docker-compose up -d
```

2. Access the container:
```bash
docker-compose exec planutils bash
```

## Stopping the Container

To stop the container:
```bash
docker-compose down
```
