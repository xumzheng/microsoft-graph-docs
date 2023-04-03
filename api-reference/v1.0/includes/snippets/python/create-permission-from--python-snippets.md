---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Permission();
requestBody.setRoles(['write', ]);

grantedToIdentitiesIdentitySet1 = IdentitySet();
grantedToIdentitiesIdentitySet1Application = Identity();
grantedToIdentitiesIdentitySet1Application.setId('89ea5c94-7736-4e25-95ad-3fa95f62b66e');

grantedToIdentitiesIdentitySet1Application.setDisplayName('Contoso Time Manager App');


grantedToIdentitiesIdentitySet1.setApplication($grantedToIdentitiesIdentitySet1Application);

grantedToIdentitiesArray []= grantedToIdentitiesIdentitySet1;
requestBody.setGrantedToIdentities(grantedToIdentitiesArray);




requestResult = graphServiceClient.sitesById('site-id').permissions().post(requestBody);


```