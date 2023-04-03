---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessageRequestBuilderGetRequestConfiguration();

queryParameters = MessageRequestBuilderGetQueryParameters();
queryParameters.select = ["subject","body","bodyPreview","uniqueBody"];

headers = [
'Prefer' => 'outlook.body-content-type="text"',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().messagesById('message-id').get(requestConfiguration);


```