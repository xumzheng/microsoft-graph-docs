---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageResourceRequest();
requestBody.setCatalogId('de9315c1-272b-4905-924b-cc112ca180c7');

accessPackageResource = AccessPackageResource();
accessPackageResource.setDisplayName('Community Outreach');

accessPackageResource.setDescription('https://contoso.sharepoint.com/sites/CSR');

accessPackageResource.setResourceType('SharePoint Online Site');

accessPackageResource.setOriginId('https://contoso.sharepoint.com/sites/CSR');

accessPackageResource.setOriginSystem('SharePointOnline');

accessPackageResourceAccessPackageResourceEnvironment = AccessPackageResourceEnvironment();
accessPackageResourceAccessPackageResourceEnvironment.setOriginId('https://contoso-admin.sharepoint.com/');


accessPackageResource.setAccessPackageResourceEnvironment($accessPackageResourceAccessPackageResourceEnvironment);

requestBody.setAccessPackageResource($accessPackageResource);
requestBody.setRequestType('AdminAdd');



requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageResourceRequests().post(requestBody);


```