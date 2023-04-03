---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

queryParameters = PrivilegedOperationEventsRequestBuilderGetQueryParameters();
queryParameters.filter = "requestType eq 'Deactivate'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.privilegedOperationEvents().get(requestConfiguration);


```