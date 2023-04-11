---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = RegistrationRequestBuilder.RegistrationRequestBuilderGetQueryParameters(
		expand = ["microsoft.graph.meetingRegistration/customQuestions"],
)

request_configuration = RegistrationRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.get(request_configuration = request_configuration)


```