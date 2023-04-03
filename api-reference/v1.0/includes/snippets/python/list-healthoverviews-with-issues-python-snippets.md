---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = HealthOverviewsRequestBuilderGetRequestConfiguration();

queryParameters = HealthOverviewsRequestBuilderGetQueryParameters();
queryParameters.expand = ["issues"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.admin().serviceAnnouncement().healthOverviews().get(requestConfiguration);


```