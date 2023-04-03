---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AttributeSetsRequestBuilderGetRequestConfiguration();

queryParameters = AttributeSetsRequestBuilderGetQueryParameters();
queryParameters.orderby = ["id"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.directory().attributeSets().get(requestConfiguration);


```