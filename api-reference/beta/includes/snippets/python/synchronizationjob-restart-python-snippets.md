---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RestartPostRequestBody()
criteria = SynchronizationJobRestartCriteria()
criteria.ResetScope(SynchronizationJobRestartScope('watermark, escrows, quarantinestate'))


request_body.criteria = criteria



await client.servicePrincipals_by_id('servicePrincipal-id').synchronization.jobs_by_id('synchronizationJob-id').restart.post(request_body = request_body, request_configuration = request_configuration)


```