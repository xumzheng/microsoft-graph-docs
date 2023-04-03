---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.filter = "isof or isof";
queryParameters.select = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.directoryObjects().delta().get(requestConfiguration);


```