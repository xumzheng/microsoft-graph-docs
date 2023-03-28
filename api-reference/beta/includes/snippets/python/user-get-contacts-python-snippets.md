---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ContactsRequestBuilderGetRequestConfiguration();

$queryParameters = new ContactsRequestBuilderGetQueryParameters();
$queryParameters.select = ["displayName","emailAddresses"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().contacts().get($requestConfiguration);


```