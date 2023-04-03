---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TemplatesRequestBuilderGetRequestConfiguration();

queryParameters = TemplatesRequestBuilderGetQueryParameters();
queryParameters.select = ["name","description","id","scenarios"];
queryParameters.filter = "scenarios has 'secureFoundation'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identity().conditionalAccess().templates().get(requestConfiguration);


```