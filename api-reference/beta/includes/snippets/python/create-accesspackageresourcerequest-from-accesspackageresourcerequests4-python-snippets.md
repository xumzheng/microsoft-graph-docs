---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = 'beedadfe-01d5-4025-910b-84abb9369997'

request_body.requestType = 'AdminAdd'

accessPackageResource = AccessPackageResource()
accessPackageResource.originId = 'c6294667-7348-4f5a-be73-9d2c65f574f3'

accessPackageResource.originSystem = 'AadGroup'


request_body.accessPackageResource = accessPackageResource


request_configuration = AccessPackageResourceRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```