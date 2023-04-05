---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RestartPostRequestBody()
criteria = SynchronizationJobRestartCriteria()
criteria.setResetScope(SynchronizationJobRestartScope('watermark, escrows, quarantinestate'))


request_body.setCriteria($criteria)

request_config = RestartRequestBuilderPostRequestConfiguration()

headers = [
	'Authorization' => 'Bearer <token>',
]

request_config.headers = headers


await client.servicePrincipals._by_id('servicePrincipal-id').synchronization.jobs._by_id('synchronizationJob-id').restart.post(request_body, request_config)


```