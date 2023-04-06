---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = RegistrationRequestBuilderGetRequestConfiguration(
request_config = RegistrationRequestBuilderGetRequestConfiguration(query_params=query_params = RegistrationRequestBuilderGetQueryParameters()
query_params.expand = ["microsoft.graph.meetingRegistration/customQuestions"]

)
query_params = RegistrationRequestBuilderGetQueryParameters()
query_params.expand = ["microsoft.graph.meetingRegistration/customQuestions"]

)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.get(request_config, headers=request_config)


```