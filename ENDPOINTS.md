# API Endpoints Documentation

This document provides a comprehensive list of API endpoints available in the Pandatory application.

## Endpoints

### Inventory

- **GET** `/api/v1/inventory`
- **POST** `/api/v1/inventory`
- **GET** `/api/v1/inventory/{{id}}`
- **PUT** `/api/v1/inventory/{{id}}`
- **DELETE** `/api/v1/inventory/{{id}}`
- **GET** `/api/v1/inventory/search`

### Shopping Sessions

- **GET** `/api/v1/shopping/sessions`
- **POST** `/api/v1/shopping/sessions`
- **GET** `/api/v1/shopping/sessions/{{id}}`
- **DELETE** `/api/v1/shopping/sessions/{{id}}`
- **POST** `/api/v1/shopping/sessions/{{sessionId}}/add-items`
- **POST** `/api/v1/shopping/sessions/{{sessionId}}/mark-purchased`
- **PUT** `/api/v1/shopping/sessions/archive/{{id}}`
- **PUT** `/api/v1/shopping/sessions/{{sessionId}}/items/{{itemId}}/quantity`

### Shopping List

- **GET** `/api/v1/shopping/list`
- **POST** `/api/v1/shopping/list`
- **GET** `/api/v1/shopping/list/{{id}}`
- **DELETE** `/api/v1/shopping/list/{{id}}`

### Dashboard

- **GET** `/api/v1/dashboard`
