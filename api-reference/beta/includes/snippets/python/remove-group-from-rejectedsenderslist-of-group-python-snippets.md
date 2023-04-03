---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RefRequestBuilderDeleteRequestConfiguration();

queryParameters = RefRequestBuilderDeleteQueryParameters();
queryParameters.id = "https://graph.microsoft.com/beta/groups/{other-group-id}";

requestConfiguration.queryParameters = queryParameters;


graphServiceClient.groupsById('group-id').rejectedSenders().ref().delete(requestConfiguration);


```