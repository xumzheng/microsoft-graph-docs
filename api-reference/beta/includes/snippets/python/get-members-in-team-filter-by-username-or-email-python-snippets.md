---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MembersRequestBuilderGetRequestConfiguration();

queryParameters = MembersRequestBuilderGetQueryParameters();
queryParameters.filter = "(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').members().get(requestConfiguration);


```