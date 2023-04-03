---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = InstalledAppsRequestBuilderGetRequestConfiguration();

queryParameters = InstalledAppsRequestBuilderGetQueryParameters();
queryParameters.expand = ["teamsAppDefinition"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.usersById('user-id').teamwork().installedApps().get(requestConfiguration);


```