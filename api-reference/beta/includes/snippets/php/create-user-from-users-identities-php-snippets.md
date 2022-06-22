---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();


$requestRequestBody->setDisplayName('John Smith');
$identitiesArray = [];

$identities1 = new ObjectIdentity();

$identities1->setSignInType('userName');
$identities1->setIssuer('contoso.onmicrosoft.com');
$identities1->setIssuerAssignedId('johnsmith');

$identitiesArray []= $identities1;

$identities2 = new ObjectIdentity();

$identities2->setSignInType('emailAddress');
$identities2->setIssuer('contoso.onmicrosoft.com');
$identities2->setIssuerAssignedId('jsmith@yahoo.com');

$identitiesArray []= $identities2;

$identities3 = new ObjectIdentity();

$identities3->setSignInType('federated');
$identities3->setIssuer('facebook.com');
$identities3->setIssuerAssignedId('5eecb0cd');

$identitiesArray []= $identities3;
$requestRequestBody->setIdentities($identitiesArray);

$passwordProfile = new PasswordProfile();
$requestRequestBody->setPasswordProfile($passwordProfile);


$passwordProfile->setPassword('password-value');
$passwordProfile->setForceChangePasswordNextSignIn(False);

$requestRequestBody->setPasswordPolicies('DisablePasswordExpiration');
$result =  $graphClient->users()->post($requestRequestBody);


```