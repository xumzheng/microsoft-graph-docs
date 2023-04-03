---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TeamTemplatesRequestBuilderGetRequestConfiguration();

queryParameters = TeamTemplatesRequestBuilderGetQueryParameters();
queryParameters.expand = ["definitions"];
queryParameters.filter = "definitions/any";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.teamwork().teamTemplates().get(requestConfiguration);


```