---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.displayName = 'John Smith'

identities_object_identity1 = ObjectIdentity()
identitiesObjectIdentity1.signInType = 'userName'

identitiesObjectIdentity1.issuer = 'contoso.onmicrosoft.com'

identitiesObjectIdentity1.issuerAssignedId = 'johnsmith'


identitiesArray []= identitiesObjectIdentity1;
identities_object_identity2 = ObjectIdentity()
identitiesObjectIdentity2.signInType = 'emailAddress'

identitiesObjectIdentity2.issuer = 'contoso.onmicrosoft.com'

identitiesObjectIdentity2.issuerAssignedId = 'jsmith@yahoo.com'


identitiesArray []= identitiesObjectIdentity2;
identities_object_identity3 = ObjectIdentity()
identitiesObjectIdentity3.signInType = 'federated'

identitiesObjectIdentity3.issuer = 'facebook.com'

identitiesObjectIdentity3.issuerAssignedId = '5eecb0cd'


identitiesArray []= identitiesObjectIdentity3;
request_body.identities(identitiesArray)


password_profile = PasswordProfile()
passwordProfile.password = 'password-value'

passwordProfile.force_change_password_next_sign_in = False


request_body.password_profile = passwordProfile
request_body.passwordPolicies = 'DisablePasswordExpiration'




result = await client.users.post(request_body = request_body)


```