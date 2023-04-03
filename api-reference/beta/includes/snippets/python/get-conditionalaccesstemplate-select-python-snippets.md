---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ConditionalAccessTemplateRequestBuilderGetRequestConfiguration();

queryParameters = ConditionalAccessTemplateRequestBuilderGetQueryParameters();
queryParameters.select = ["details"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identity().conditionalAccess().templatesById('conditionalAccessTemplate-id').get(requestConfiguration);


```