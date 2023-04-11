---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PassiveDnsRecordRequestBuilderGetRequestConfiguration(
)


result = await client.security.threatIntelligence.passiveDnsRecords_by_id('passiveDnsRecord-id').get()


```