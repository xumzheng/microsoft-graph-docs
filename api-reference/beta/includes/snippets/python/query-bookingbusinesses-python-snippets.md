---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = BookingBusinessesRequestBuilderGetRequestConfiguration();

query_params = BookingBusinessesRequestBuilderGetQueryParameters();
query_params.query = "Adventure";

request_config.queryParameters = query_params;


result = awaitclient.bookingBusinesses().get(request_config);


```