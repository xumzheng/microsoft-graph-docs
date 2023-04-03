---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TeamsAppInstallationRequestBuilderGetRequestConfiguration();

queryParameters = TeamsAppInstallationRequestBuilderGetQueryParameters();
queryParameters.expand = ["teamsAppDefinition"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamsById('team-id').installedAppsById('teamsAppInstallation-id').get(requestConfiguration);


```