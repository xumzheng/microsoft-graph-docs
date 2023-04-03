---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessageRequestBuilderGetRequestConfiguration();

queryParameters = MessageRequestBuilderGetQueryParameters();
queryParameters.expand = ["extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().messagesById('message-id').get(requestConfiguration);


```