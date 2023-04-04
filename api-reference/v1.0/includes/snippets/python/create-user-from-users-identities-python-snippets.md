---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = User()
request_body.setDisplayName('John Smith')

identitiesObjectIdentity1 = ObjectIdentity()
identitiesObjectIdentity1.setSignInType('userName')

identitiesObjectIdentity1.setIssuer('contoso.onmicrosoft.com')

identitiesObjectIdentity1.setIssuerAssignedId('johnsmith')


identitiesArray []= identitiesObjectIdentity1;
identitiesObjectIdentity2 = ObjectIdentity()
identitiesObjectIdentity2.setSignInType('emailAddress')

identitiesObjectIdentity2.setIssuer('contoso.onmicrosoft.com')

identitiesObjectIdentity2.setIssuerAssignedId('jsmith@yahoo.com')


identitiesArray []= identitiesObjectIdentity2;
identitiesObjectIdentity3 = ObjectIdentity()
identitiesObjectIdentity3.setSignInType('federated')

identitiesObjectIdentity3.setIssuer('facebook.com')

identitiesObjectIdentity3.setIssuerAssignedId('5eecb0cd')


identitiesArray []= identitiesObjectIdentity3;
request_body.setIdentities(identitiesArray)


passwordProfile = PasswordProfile()
passwordProfile.setPassword('password-value')

passwordProfile.setForceChangePasswordNextSignIn(false)


request_body.setPasswordProfile($passwordProfile)
request_body.setPasswordPolicies('DisablePasswordExpiration')



result = await client.users.post(request_body)


```