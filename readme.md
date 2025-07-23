# Microsoft SQL Server on PipeOps

Deploy Microsoft SQL Server 2022 Developer Edition on PipeOps with persistent storage and secure configuration.

## Overview

This addon provides a fully configured Microsoft SQL Server instance that's ready for development and testing workloads. It includes persistent storage for your databases and secure credential management.

## Features

- **Microsoft SQL Server 2022** Developer Edition
- **Persistent Storage** - 1GB volume mounted at `/var/opt/mssql`
- **Secure Credentials** - Auto-generated passwords for SA and root users
- **Network Access** - Accessible on port 1433
- **Pre-configured Database** - Default database named `pipeops`
- **EULA Acceptance** - Automatically accepts Microsoft's End-User License Agreement

## Quick Start

1. **Deploy from PipeOps Marketplace**
   - Navigate to the PipeOps dashboard
   - Go to the Addons marketplace
   - Search for "Microsoft SQL Server"
   - Click "Deploy"

2. **Configuration**
   - The addon comes pre-configured with sensible defaults
   - Database credentials are automatically generated
   - No additional setup required

## Environment Variables

| Variable | Description | Default Value |
|----------|-------------|---------------|
| `PORT` | SQL Server port | `1433` |
| `MSSQL_TCP_PORT` | TCP port for SQL Server | `1433` |
| `MSSQL_SERVER` | Server host address | `0.0.0.0` |
| `MSSQL_DATABASE` | Default database name | `pipeops` |
| `MSSQL_USERNAME` | Default username | `pipeops_user` |
| `MSSQL_SA_PASSWORD` | SA user password | Auto-generated (25 chars) |
| `MSSQL_ROOT_PASSWORD` | Root password | Auto-generated (32 chars) |
| `MSSQL_PID` | SQL Server edition | `Developer` |
| `ACCEPT_EULA` | EULA acceptance | `Y` |
| `MSSQL_URL` | Connection string | Auto-generated |
