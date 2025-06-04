# Hello World API

This test project is a simple Node.js application that sets up an Express server and responds with "Hello, World!" when accessed. It is designed to be deployed to Azure using GitHub Actions.

## Project Structure

```
hello-world-api
├── src
│   └── index.js        # Entry point of the application
├── .github
│   └── workflows
│       └── azure-deploy.yml  # GitHub Actions workflow for Azure deployment
├── package.json        # npm configuration file
└── README.md           # Project documentation
```

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd hello-world-api
   ```

2. **Install dependencies:**

   Make sure you have Node.js and npm installed. Then run:

   ```bash
   npm install
   ```

3. **Run the application:**

   You can start the server by running:

   ```bash
   npm start
   ```

   The server will be available at `http://localhost:3000`, and you should see "Hello, World!" when you access this URL.

## Deployment to Azure

This project is set up to deploy automatically to Azure using GitHub Actions. The workflow is defined in the `.github/workflows/azure-deploy.yml` file. 

Whenever you push changes to the `main` branch, the workflow will trigger and deploy the application to Azure.

### Prerequisites

- An Azure account
- Azure CLI installed and configured
- A resource group and web app created in Azure

### Configuration

Make sure to update the `azure-deploy.yml` file with your Azure credentials and app details.

## License

This project is licensed under the MIT License. See the LICENSE file for details.