---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = BookingBusinessesRequestBuilderGetRequestConfiguration(
query_params = BookingBusinessesRequestBuilderGetQueryParameters()
query_params.query = "Adventure"

)


result = await client.bookingBusinesses.get(request_config)


```