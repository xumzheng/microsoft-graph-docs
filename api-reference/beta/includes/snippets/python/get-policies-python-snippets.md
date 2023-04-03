---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PoliciesRequestBuilderGetRequestConfiguration();

queryParameters = PoliciesRequestBuilderGetQueryParameters();
queryParameters.filter = "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identity().conditionalAccess().policies().get(requestConfiguration);


```