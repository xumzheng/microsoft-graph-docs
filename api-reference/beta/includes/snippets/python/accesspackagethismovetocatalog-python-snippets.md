---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MoveToCatalogPostRequestBody()
request_body.setCatalogId('3301434b-99bd-46be-923b-d762c30c8e8b')



await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').moveToCatalog.post(request_body, headers=)


```