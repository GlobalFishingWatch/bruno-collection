# Bruno API Collections

This repository contains [Bruno](https://www.usebruno.com/) API collections for testing and exploring Global Fishing Watch (GFW) APIs.

## 📁 Collections

### GFW API

The main collection for interacting with the **Global Fishing Watch API v3**. This comprehensive collection covers all major API endpoints for tracking fishing activity, vessel data, and marine analytics.

#### Endpoints Include:

| Category                | Description                                        |
| ----------------------- | -------------------------------------------------- |
| **4Wings**              | Tile generation, statistics, and temporal datasets |
| **Auth**                | Authentication, user management, and token refresh |
| **Bulk Reports**        | Create and manage bulk report operations           |
| **Context Layers**      | Geographic and contextual map layers               |
| **Datasets**            | Dataset CRUD operations and DOI publishing         |
| **Dataviews**           | Data visualization configurations                  |
| **Download**            | Dataset file downloads                             |
| **Events**              | Fishing events, encounters, and activity data      |
| **Insights**            | Vessel and vessel group analytics                  |
| **Reports**             | Report generation and management                   |
| **Tracks**              | Vessel track data and downloads                    |
| **User Context Layers** | Custom user-uploaded layers                        |
| **User Groups**         | User group management                              |
| **Vessel Groups**       | Vessel group CRUD operations                       |
| **Vessels**             | Vessel search, autocomplete, and details           |
| **Workspaces**          | Workspace management for map configurations        |

### fishing-map

A smaller collection for local development and testing of the fishing map application.

## 🚀 Getting Started

### Prerequisites

1. Install [Bruno](https://www.usebruno.com/) - an open-source API client
2. Obtain an API token from [Global Fishing Watch](https://globalfishingwatch.org/our-apis/)

### Setup

1. Clone this repository:

   ```bash
   git clone <repository-url>
   cd bruno
   ```

2. Open Bruno and select **Open Collection**

3. Navigate to the collection folder you want to use (e.g., `GFW API`)

4. Configure your environment:
   - Select either **Development** or **Production** environment
   - Set your `token` secret variable with your GFW API token

### Environments

| Environment     | Base URL                                         |
| --------------- | ------------------------------------------------ |
| **Production**  | `https://gateway.api.globalfishingwatch.org`     |
| **Development** | `https://gateway.api.dev.globalfishingwatch.org` |

## 🔐 Authentication

All GFW API requests require a Bearer token in the Authorization header:

```
Authorization: Bearer <your-token>
```

The token is automatically included via the collection-level headers when you set the `token` secret variable in your environment.

## 📚 Resources

- [Global Fishing Watch API Documentation](https://globalfishingwatch.org/our-apis/documentation)
- [Bruno Documentation](https://docs.usebruno.com/)
- [Global Fishing Watch](https://globalfishingwatch.org/)

## 🤝 Contributing

Feel free to add new requests, update existing ones, or improve documentation by submitting a pull request.

## 📄 License

This project is for internal use with Global Fishing Watch APIs.
