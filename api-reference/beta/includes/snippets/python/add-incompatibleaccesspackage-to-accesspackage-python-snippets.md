---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate();
request_body.set@odataid('https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2');



await client.identityGovernance.entitlementManagement.accessPackagesById('accessPackage-id').incompatibleAccessPackages.ref.post(request_body);


```