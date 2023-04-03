---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MembersRequestBuilderGetRequestConfiguration();

queryParameters = MembersRequestBuilderGetQueryParameters();
queryParameters.filter = "roles/any";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').members().get(requestConfiguration);


```