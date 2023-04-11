---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.displayName = 'John Smith'

identitiesObjectIdentity1 = ObjectIdentity()
identitiesObjectIdentity1.signInType = 'userName'

identitiesObjectIdentity1.issuer = 'contoso.onmicrosoft.com'

identitiesObjectIdentity1.issuerAssignedId = 'johnsmith'


identitiesArray []= identitiesObjectIdentity1;
identitiesObjectIdentity2 = ObjectIdentity()
identitiesObjectIdentity2.signInType = 'emailAddress'

identitiesObjectIdentity2.issuer = 'contoso.onmicrosoft.com'

identitiesObjectIdentity2.issuerAssignedId = 'jsmith@yahoo.com'


identitiesArray []= identitiesObjectIdentity2;
identitiesObjectIdentity3 = ObjectIdentity()
identitiesObjectIdentity3.signInType = 'federated'

identitiesObjectIdentity3.issuer = 'facebook.com'

identitiesObjectIdentity3.issuerAssignedId = '5eecb0cd'


identitiesArray []= identitiesObjectIdentity3;
request_body.identities(identitiesArray)


passwordProfile = PasswordProfile()
passwordProfile.password = 'password-value'

passwordProfile.forceChangePasswordNextSignIn = false


request_body.passwordProfile = passwordProfile
request_body.passwordPolicies = 'DisablePasswordExpiration'



request_configuration = UsersRequestBuilderPostRequestConfiguration(
)


result = await client.users.post(request_body = request_body)


```