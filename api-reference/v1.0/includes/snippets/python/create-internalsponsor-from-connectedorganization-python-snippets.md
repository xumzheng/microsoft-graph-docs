---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/users/{id}');



awaitclient.identityGovernance().entitlementManagement().connectedOrganizationsById('connectedOrganization-id').internalSponsors().ref().post(requestBody);


```