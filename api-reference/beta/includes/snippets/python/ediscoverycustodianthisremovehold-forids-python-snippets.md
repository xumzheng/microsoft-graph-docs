---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RemoveHoldPostRequestBody()
request_body.setIds(['7f697316-43ed-48e1-977f-261be050db93', 'b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8', ])



await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').custodians.securityremoveHold.post(request_body)


```