---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.catalogId = '26ac0c0a-08bc-4a7b-a313-839f58044ba5'

request_body.requestType = 'AdminAdd'

request_body.justification = ''

accessPackageResource = AccessPackageResource()
accessPackageResource.displayName = 'Sales'

accessPackageResource.description = 'https://contoso.sharepoint.com/sites/Sales'

accessPackageResource.url = 'https://contoso.sharepoint.com/sites/Sales'

accessPackageResource.resourceType = 'SharePoint Online Site'

accessPackageResource.originId = 'https://contoso.sharepoint.com/sites/Sales'

accessPackageResource.originSystem = 'SharePointOnline'


request_body.accessPackageResource = accessPackageResource



result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body = request_body)


```