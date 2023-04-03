---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessageRequestBuilderGetRequestConfiguration();

queryParameters = MessageRequestBuilderGetQueryParameters();
queryParameters.expand = ["singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().messagesById('message-id').get(requestConfiguration);


```