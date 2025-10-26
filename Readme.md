# API Gateway
A Spring Cloud Gateway implementation for the E-Commerce platform that handles routing, authentication, and global configuration.

## Project Structure
```
API-GATEWAY/
├── src/main/java/com/e_commence/api_gateway/
│   ├── config/
│   │   ├── AuthGlobalFilter.java      # Global authentication filter
│   │   ├── ConsGlobalConfig.java      # Consumer global configuration
│   │   ├── GatewayConfig.java         # Gateway routing configuration
│   │   ├── GatewayErrorHandlerConfig.java # Error handling configuration
│   │   └── ApiGatewayApplication.java # Main application class
│   └── resources/
│       ├── .env                       # Environment variables (not tracked in git)
│       ├── .env.example               # Environment variables template
│       └── application.properties     # Spring application configuration
├── target/
│   ├── classes/
│   ├── generated-sources/
│   ├── generated-test-sources/
│   ├── maven-archiver/
│   ├── maven-status/
│   ├── test-classes/
│   └── api-gateway-1.0.0.jar         # Built application JAR
├── .gitattributes
├── .gitignore
├── mvnw                            # Maven wrapper (Unix/Linux)
├── mvnw.cmd                        # Maven wrapper (Windows)
└── pom.xml                         # Maven dependencies and build configuration
```

## Features
- Request Routing: Intelligent routing to various microservices.
- Authentication: Global authentication filter for securing endpoints.
- Error Handling: Centralized error handling configuration.
- Configuration Management: Externalized configuration support.
- CORS Configuration: Cross-origin resource sharing setup.