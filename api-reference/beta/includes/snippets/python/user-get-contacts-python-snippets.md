---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ContactsRequestBuilderGetRequestConfiguration();

query_params = ContactsRequestBuilderGetQueryParameters();
query_params.select = ["displayName","emailAddresses"];

request_config.queryParameters = query_params;


result = awaitclient.me().contacts().get(request_config);


```