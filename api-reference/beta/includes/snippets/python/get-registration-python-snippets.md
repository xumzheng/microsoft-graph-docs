---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RegistrationRequestBuilderGetRequestConfiguration(
request_configuration = RegistrationRequestBuilderGetRequestConfiguration(query_params=query_params = RegistrationRequestBuilderGetQueryParameters()
query_params['expand'] = ["microsoft.graph.meetingRegistration/customQuestions"]

)
query_params = RegistrationRequestBuilderGetQueryParameters()
query_params['expand'] = ["microsoft.graph.meetingRegistration/customQuestions"]

)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.get(request_configuration)


```