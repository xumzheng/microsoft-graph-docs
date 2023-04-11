---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = 'de9315c1-272b-4905-924b-cc112ca180c7'

accessPackageResource = AccessPackageResource()
accessPackageResource.displayName = 'Community Outreach'

accessPackageResource.description = 'https://contoso.sharepoint.com/sites/CSR'

accessPackageResource.resourceType = 'SharePoint Online Site'

accessPackageResource.originId = 'https://contoso.sharepoint.com/sites/CSR'

accessPackageResource.originSystem = 'SharePointOnline'

additionalData = [
'accessPackageResourceEnvironment@odata.bind' => 'accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57', 
];
accessPackageResource.additionaldata(additionalData)



request_body.accessPackageResource = accessPackageResource
request_body.requestType = 'AdminAdd'




result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```