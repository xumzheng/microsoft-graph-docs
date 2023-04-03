---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.select = ["displayName","jobTitle","mail"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.contacts().delta().get(requestConfiguration);


```