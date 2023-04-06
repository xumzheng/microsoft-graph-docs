---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MutePostRequestBody()
request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')


request_config = MuteRequestBuilderPostRequestConfiguration(
request_config = MuteRequestBuilderPostRequestConfiguration(query_params=)


result = await client.communications.calls_by_id('call-id').participants_by_id('participant-id').mute.post(request_body, headers=)


```