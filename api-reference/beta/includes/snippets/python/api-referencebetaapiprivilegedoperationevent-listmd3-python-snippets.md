---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

queryParameters = PrivilegedOperationEventsRequestBuilderGetQueryParameters();
queryParameters.filter = "(creationDateTime ge 2017-06-25T07:00:00Z) and ";
queryParameters.count = true;
queryParameters.orderby = ["creationDateTime desc"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.privilegedOperationEvents().get(requestConfiguration);


```