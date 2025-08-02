# Harbor Parking API Documentation

Complete REST API documentation for the Harbor Parking application. This documentation provides comprehensive guidance for integrating with the Harbor Parking API to manage parking spot sharing within residential communities.

## Features

- **Authentication** - JWT-based authentication with Supabase
- **Parking Spots** - CRUD operations for parking spot management
- **Availabilities** - Time-based availability window management
- **Claims** - Parking spot reservation system
- **Dashboard** - User dashboard with statistics and recent activity

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview the documentation locally:

```bash
npm i -g mint
```

Start the development server:

```bash
mint dev
```

View the documentation at `http://localhost:3000`.

## API Overview

The Harbor Parking API is a REST API that enables parking spot sharing functionality. Key features include:

- User profile management
- Parking spot registration and verification
- Availability scheduling
- Spot claiming and reservation
- Real-time dashboard data

## Base URL

```
https://harbor-parking.vercel.app/api
```

## Authentication

All API endpoints require JWT authentication. See the [Authentication Guide](https://docs.harbor-parking.com/authentication) for details.

## Links

- **Harbor Parking App**: https://harbor-parking.vercel.app
- **GitHub Repository**: https://github.com/ylapscher/harbor-parking
- **API Documentation**: https://docs.harbor-parking.com
