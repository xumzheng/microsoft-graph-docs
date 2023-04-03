---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessagesRequestBuilderGetRequestConfiguration();

queryParameters = MessagesRequestBuilderGetQueryParameters();
queryParameters.top = 2;
queryParameters.filter = "lastModifiedDateTime gt 2021-03-17T07:13:28.000z";
queryParameters.orderby = ["createdDateTime desc"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.usersById('user-id').chatsById('chat-id').messages().get(requestConfiguration);


```