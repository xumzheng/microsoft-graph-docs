---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServiceHealthRequestBuilderGetRequestConfiguration();

queryParameters = ServiceHealthRequestBuilderGetQueryParameters();
queryParameters.expand = ["issues"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.admin().serviceAnnouncement().healthOverviewsById('serviceHealth-id').get(requestConfiguration);


```