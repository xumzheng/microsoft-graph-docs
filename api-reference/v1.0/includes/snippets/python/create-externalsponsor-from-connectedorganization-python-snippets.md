---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/v1.0/users/{id}');



await client.identityGovernance().entitlementManagement().connectedOrganizationsById('connectedOrganization-id').externalSponsors().ref().post(requestBody);


```