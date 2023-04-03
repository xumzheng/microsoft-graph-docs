---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = DeltaRequestBuilderGetRequestConfiguration();

queryParameters = DeltaRequestBuilderGetQueryParameters();
queryParameters.select = ["displayName","description","mailNickname"];

headers = [
'Prefer' => 'return=minimal',
];

requestConfiguration.queryParameters = queryParameters;
requestConfiguration.headers = headers;


requestResult = graphServiceClient.groups().delta().get(requestConfiguration);


```