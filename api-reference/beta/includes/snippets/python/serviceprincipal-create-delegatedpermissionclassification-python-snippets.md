---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DelegatedPermissionClassification()
request_body.setPermissionId('e1fe6dd8-ba31-4d61-89e7-88639da4683d')

request_body.setPermissionName('User.Read')

request_body.setClassification(PermissionClassificationType('low'))



result = await client.servicePrincipalsby_id('servicePrincipal-id')_delegatedPermissionClassifications.post(request_body)


```