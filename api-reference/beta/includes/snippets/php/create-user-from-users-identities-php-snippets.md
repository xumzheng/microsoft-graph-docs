---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();


$requestRequestBody->setDisplayName('John Smith');
$identitiesArray = [];

$identitiesidentities1 = new ObjectIdentity();

$identitiesidentities1->setSignInType('userName');
$identitiesidentities1->setIssuer('contoso.onmicrosoft.com');
$identitiesidentities1->setIssuerAssignedId('johnsmith');

$identitiesArray []= $identitiesidentities1;

$identitiesidentities2 = new ObjectIdentity();

$identitiesidentities2->setSignInType('emailAddress');
$identitiesidentities2->setIssuer('contoso.onmicrosoft.com');
$identitiesidentities2->setIssuerAssignedId('jsmith@yahoo.com');

$identitiesArray []= $identitiesidentities2;

$identitiesidentities3 = new ObjectIdentity();

$identitiesidentities3->setSignInType('federated');
$identitiesidentities3->setIssuer('facebook.com');
$identitiesidentities3->setIssuerAssignedId('5eecb0cd');

$identitiesArray []= $identitiesidentities3;
$requestRequestBody->setIdentities($identitiesArray);

$passwordProfile = new PasswordProfile();
$requestRequestBody->setPasswordProfile($passwordProfile);


$passwordProfile->setPassword('password-value');
$passwordProfile->setForceChangePasswordNextSignIn(False);

$requestRequestBody->setPasswordPolicies('DisablePasswordExpiration');
$result =  $graphClient->users()->post($requestRequestBody);


```