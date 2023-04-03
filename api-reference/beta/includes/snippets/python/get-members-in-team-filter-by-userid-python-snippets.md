---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MembersRequestBuilderGetRequestConfiguration();

queryParameters = MembersRequestBuilderGetQueryParameters();
queryParameters.filter = "(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').members().get(requestConfiguration);


```