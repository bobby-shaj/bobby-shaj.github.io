# StockTracker Web API

This document provides information about the API, including endpoints, authentication, and usage examples.

## Introduction

This API services requests for the two main features of the StockTracker Web Application; Stocks and SEC Filings. 
It is built using .NET Core and follows RESTful principles.

## Getting Started

### Prerequisites

* [.NET Runtime](https://dotnet.microsoft.com/download)
* MS SQL Server 2019

### Installation

1. Clone the repository: `git clone [repository URL]`
2. Navigate to the project directory: `cd [project directory]`
3. Restore dependencies: `dotnet restore`
4. Build the project: `dotnet build`
5. Run the API: `dotnet run`

## API Endpoints
* [Stocks](./Features/Stocks.md)
* [Filings](./Features/Filings.md)