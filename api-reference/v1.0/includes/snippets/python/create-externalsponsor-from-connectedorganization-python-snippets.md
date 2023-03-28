---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReferenceCreate();
$requestBody->set@odataid('https://graph.microsoft.com/v1.0/users/{id}');



$graphServiceClient->identityGovernance()->entitlementManagement()->connectedOrganizationsById('connectedOrganization-id')->externalSponsors()->ref()->post($requestBody);


```