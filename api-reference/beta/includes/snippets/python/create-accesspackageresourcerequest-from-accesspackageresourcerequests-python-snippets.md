---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageResourceRequest();
request_body.setCatalogId('26ac0c0a-08bc-4a7b-a313-839f58044ba5');

request_body.setRequestType('AdminAdd');

request_body.setJustification('');

accessPackageResource = AccessPackageResource();
accessPackageResource.setDisplayName('Sales');

accessPackageResource.setDescription('https://contoso.sharepoint.com/sites/Sales');

accessPackageResource.setUrl('https://contoso.sharepoint.com/sites/Sales');

accessPackageResource.setResourceType('SharePoint Online Site');

accessPackageResource.setOriginId('https://contoso.sharepoint.com/sites/Sales');

accessPackageResource.setOriginSystem('SharePointOnline');


request_body.setAccessPackageResource($accessPackageResource);


result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body);


```