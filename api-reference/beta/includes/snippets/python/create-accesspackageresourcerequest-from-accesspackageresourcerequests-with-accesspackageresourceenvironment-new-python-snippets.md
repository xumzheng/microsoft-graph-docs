---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageResourceRequest()
request_body.setCatalogId('de9315c1-272b-4905-924b-cc112ca180c7')

accessPackageResource = AccessPackageResource()
accessPackageResource.setDisplayName('Community Outreach')

accessPackageResource.setDescription('https://contoso.sharepoint.com/sites/CSR')

accessPackageResource.setResourceType('SharePoint Online Site')

accessPackageResource.setOriginId('https://contoso.sharepoint.com/sites/CSR')

accessPackageResource.setOriginSystem('SharePointOnline')

accessPackageResourceAccessPackageResourceEnvironment = AccessPackageResourceEnvironment()
accessPackageResourceAccessPackageResourceEnvironment.setOriginId('https://contoso-admin.sharepoint.com/')


accessPackageResource.setAccessPackageResourceEnvironment($accessPackageResourceAccessPackageResourceEnvironment)

request_body.setAccessPackageResource($accessPackageResource)
request_body.setRequestType('AdminAdd')



result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body)


```