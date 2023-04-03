---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.token = "1230919asd190410jlka";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.sitesById('site-id').listsById('list-id').items().delta().get(requestConfiguration);


```