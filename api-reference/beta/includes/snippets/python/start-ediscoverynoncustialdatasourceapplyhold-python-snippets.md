---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyHoldPostRequestBody()
request_body.setIds(['39333641443238353535383731453339', '46333131344239353834433430454335', ])



await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources.securityapplyHold.post(request_body, headers=)


```