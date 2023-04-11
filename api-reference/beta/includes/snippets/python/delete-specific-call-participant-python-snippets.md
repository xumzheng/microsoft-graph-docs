---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = ParticipantRequestBuilderDeleteRequestConfiguration(
)


await client.communications.calls_by_id('call-id').participants_by_id('participant-id').delete()


```