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

request_config = RestartRequestBuilderPostRequestConfiguration(
request_config = RestartRequestBuilderPostRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


await client.servicePrincipals_by_id('servicePrincipal-id').synchronization.jobs_by_id('synchronizationJob-id').restart.post(request_body, request_config, headers=request_config)


```