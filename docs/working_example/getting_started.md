This section covers creating a working Data Vault 2.0 implementation using the dbtvault-scalefree package for dbt. We will use the [Stackoverflow Public Dataset hosted at the Google BigQuery Marketplace](https://console.cloud.google.com/marketplace/product/stack-exchange/stack-overflow). 

This instruction will only focus on basic aspects of the dbtvault-scalefree package. You will find detailed instructions for each feature of dbtvault-scalefree inside the [tutorial section](../tutorial/turorial_landing.md). 

This example will include: 

- Setting up a dbt project
- Exploring parts of the Stackoverflow dataset and model a Data Vault 2.0 solution for it
- Connecting your dbt project to the Stackoverflow dataset
- Creating a staging layer for hash calculation
- Creating a Raw Vault including Hubs, Links and Satellites using dbtvault-scalefree
- Creating a PIT table inside the Business Vault

## Pre-Requisites

The following requirements are only needed, if you plan to follow this tutorial and create your version of our example project. 

1. Brief knowledge of Data Vault 2.0. Find info [here](https://www.scalefree.com/what-is-data-vault/).

2. A Google Cloud Services (GCS) trial account. Get 1 TB of queries per month for BigQuery [here](https://cloud.google.com/free). 