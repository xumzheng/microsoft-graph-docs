---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = BookingBusinessesRequestBuilderGetRequestConfiguration();

queryParameters = BookingBusinessesRequestBuilderGetQueryParameters();
queryParameters.query = "Adventure";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.solutions().bookingBusinesses().get(requestConfiguration);


```