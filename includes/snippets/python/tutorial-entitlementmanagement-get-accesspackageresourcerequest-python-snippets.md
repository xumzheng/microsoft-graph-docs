---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = 'cec5d6ab-c75d-47c0-9c1c-92e89f66e384'

request_body.requestType = 'AdminAdd'

request_body.justification = ''

accessPackageResource = AccessPackageResource()
accessPackageResource.displayName = 'Marketing resources'

accessPackageResource.description = 'Marketing group'

accessPackageResource.resourceType = 'AadGroup'

accessPackageResource.originId = 'e93e24d1-2b65-4a6c-a1dd-654a12225487'

accessPackageResource.originSystem = 'AadGroup'


request_body.accessPackageResource = accessPackageResource


request_configuration = AccessPackageResourceRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```