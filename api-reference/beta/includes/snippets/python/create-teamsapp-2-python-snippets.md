---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TeamsAppsRequestBuilderPostRequestConfiguration();

queryParameters = TeamsAppsRequestBuilderPostQueryParameters();
queryParameters.requiresreview = true;

requestConfiguration.queryParameters = queryParameters;


graphServiceClient.appCatalogs().teamsApps().post(requestConfiguration);


```