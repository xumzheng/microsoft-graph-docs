---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = MessagesRequestBuilderGetRequestConfiguration();

query_params = MessagesRequestBuilderGetQueryParameters;
query_params.orderby = ["from/emailAddress/name desc","subject"];

request_config.queryParameters = query_params;


result = await client.me().mailFoldersById('mailFolder-id').messages().get(request_config);


```