---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = MessageRequestBuilderGetRequestConfiguration();

query_params = MessageRequestBuilderGetQueryParameters();
query_params.expand = ["extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"];

request_config.queryParameters = query_params;


result = awaitclient.me().messagesById('message-id').get(request_config);


```