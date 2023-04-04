---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = MessageRequestBuilderGetRequestConfiguration();

query_params = MessageRequestBuilderGetQueryParameters;
query_params.expand = ["singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')"];

request_config.queryParameters = query_params;


result = await client.me().messagesById('message-id').get(request_config);


```