---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/groups/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2');



awaitclient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').incompatibleGroups().ref().post(requestBody);


```