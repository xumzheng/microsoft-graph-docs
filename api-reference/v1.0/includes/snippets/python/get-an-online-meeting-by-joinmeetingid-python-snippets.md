---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OnlineMeetingsRequestBuilderGetRequestConfiguration(
query_params = OnlineMeetingsRequestBuilderGetQueryParameters()
query_params.filter = "joinMeetingIdSettings/joinMeetingId eq '1234567890'"

)


result = await client.me.onlineMeetings.get(request_config)


```