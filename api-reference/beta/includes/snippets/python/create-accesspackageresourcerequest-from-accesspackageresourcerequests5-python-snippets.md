---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = 'beedadfe-01d5-4025-910b-84abb9369997'

request_body.requestType = 'AdminRemove'

accessPackageResource = AccessPackageResource()
accessPackageResource.id = '354078e5-dbce-4894-8af4-0ab274d41662'


request_body.accessPackageResource = accessPackageResource



result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```