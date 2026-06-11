# CST8917 - Serverless Applications

##  Database Choice
#### Lab 1: Create and Deploy Your First Azure Function

#### Student Information

* Name: Xinyi Zhao
* Student Number: 040953633
* Course: CST8917 - Serverless Applications
* Lab: Lab 1


## 1. Selected Database

Azure Cosmos DB for NoSQL (Serverless)

## 2. Justification

Azure Cosmos DB was selected for this project because the Text Analyzer application generates JSON-based analysis results that can be stored directly as documents. Since the data structure is flexible, a NoSQL database is a good fit and does not require a predefined schema.

Cosmos DB also integrates well with Azure Functions through the Azure Cosmos Python SDK, making it easy to store and retrieve analysis results. In addition, the Serverless capacity mode supports pay-per-use pricing, which is suitable for small projects and student environments.

## 3. Alternatives Considered

#### Azure Table Storage

Azure Table Storage is a low-cost option for storing structured data. However, it provides more limited querying capabilities and is less suitable for storing nested JSON documents.

#### Azure SQL Database

Azure SQL Database offers powerful relational database features and SQL querying. However, it requires a fixed schema and additional database design, which is unnecessary for this document-oriented application.

#### Azure Blob Storage

Azure Blob Storage can store JSON files, but it is designed for file storage rather than querying individual records. Retrieving and filtering analysis results would be less efficient.

## 4. Cost Considerations

The Serverless tier of Azure Cosmos DB charges only for the request units (RUs) consumed and the amount of data stored. Because this project generates a relatively small number of requests, the expected cost is very low and can typically be covered by Azure for Students credits.