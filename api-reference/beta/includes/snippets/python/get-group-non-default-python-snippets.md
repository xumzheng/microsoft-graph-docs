---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = GroupRequestBuilderGetRequestConfiguration();

queryParameters = GroupRequestBuilderGetQueryParameters();
queryParameters.select = ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.groupsById('group-id').get(requestConfiguration);


```