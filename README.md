# CST8917 - Serverless Applications

#### Lab 1: Create and Deploy Your First Azure Function

#### Student Information

* Name: Xinyi Zhao
* Student Number: 040953633
* Course: CST8917 - Serverless Applications
* Lab: Lab 1

------

## Project Overview

This project implements a serverless Text Analyzer application using Azure Functions and Azure Cosmos DB.

The application analyzes user-provided text, stores analysis results in Azure Cosmos DB, and provides an endpoint to retrieve previously stored analysis records.

------

### Technologies Used

* Azure Functions
* Python 3.12
* Azure Cosmos DB for NoSQL (Serverless)
* Azure Functions Core Tools
* Visual Studio Code

------

### Installation

#### Install required dependencies:

`pip install -r requirements.txt`

#### Local Configuration

Create a local.settings.json file and configure:

```
* COSMOS_ENDPOINT
* COSMOS_KEY
* COSMOS_DATABASE
* COSMOS_CONTAINER
```

#### Run Locally

`func start`

#### API Endpoints

`TextAnalyzer`

Analyzes text and stores results in Cosmos DB.

Example:

`http://localhost:7071/api/TextAnalyzer?text=Hello%20World`

#### GetAnalysisHistory

Retrieves stored analysis records.

Example:

`http://localhost:7071/api/GetAnalysisHistory`

Limit Example:

`http://localhost:7071/api/GetAnalysisHistory?limit=5`

------

### Database Information

**Database:** TextAnalyzerDB

**Container:** AnalysisResults

**Database Service:** Azure Cosmos DB for NoSQL (Serverless)

------

### Demo Video

https://youtu.be/UpbouYtihUA