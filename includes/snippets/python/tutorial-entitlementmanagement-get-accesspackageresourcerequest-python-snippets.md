---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.setCatalogId('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')

request_body.setRequestType('AdminAdd')

request_body.setJustification('')

accessPackageResource = AccessPackageResource()
accessPackageResource.setDisplayName('Marketing resources')

accessPackageResource.setDescription('Marketing group')

accessPackageResource.setResourceType('AadGroup')

accessPackageResource.setOriginId('e93e24d1-2b65-4a6c-a1dd-654a12225487')

accessPackageResource.setOriginSystem('AadGroup')


request_body.setAccessPackageResource($accessPackageResource)

request_config = AccessPackageResourceRequestsRequestBuilderPostRequestConfiguration(
request_config = AccessPackageResourceRequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body, headers=)


```