---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantAppManagementPolicy();


$requestRequestBody->setIsEnabled(True);

$applicationRestrictions = new AppManagementConfiguration();
$requestRequestBody->setApplicationRestrictions($applicationRestrictions);


$passwordCredentialsArray = [];

$passwordCredentials1 = new PasswordCredentialConfiguration();

$passwordCredentials1->setRestrictionType(new AppCredentialRestrictionType('passwordAddition'));
$passwordCredentials1->setMaxLifetime(null);
$passwordCredentials1->setRestrictForAppsCreatedAfterDateTime(new DateTime("2021-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentials1;

$passwordCredentials2 = new PasswordCredentialConfiguration();

$passwordCredentials2->setRestrictionType(new AppCredentialRestrictionType('passwordLifetime'));
$passwordCredentials2->setMaxLifetime('P4DT12H30M5S');
$passwordCredentials2->setRestrictForAppsCreatedAfterDateTime(new DateTime("2017-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentials2;

$passwordCredentials3 = new PasswordCredentialConfiguration();

$passwordCredentials3->setRestrictionType(new AppCredentialRestrictionType('symmetricKeyAddition'));
$passwordCredentials3->setMaxLifetime(null);
$passwordCredentials3->setRestrictForAppsCreatedAfterDateTime(new DateTime("2021-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentials3;

$passwordCredentials4 = new PasswordCredentialConfiguration();

$passwordCredentials4->setRestrictionType(new AppCredentialRestrictionType('customPasswordAddition'));
$passwordCredentials4->setMaxLifetime(null);
$passwordCredentials4->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentials4;

$passwordCredentials5 = new PasswordCredentialConfiguration();

$passwordCredentials5->setRestrictionType(new AppCredentialRestrictionType('symmetricKeyLifetime'));
$passwordCredentials5->setMaxLifetime('P40D');
$passwordCredentials5->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentials5;
$applicationRestrictions->setPasswordCredentials($passwordCredentialsArray);
$keyCredentialsArray = [];

$keyCredentials1 = new KeyCredentialConfiguration();

$keyCredentials1->setRestrictionType(new AppKeyCredentialRestrictionType('asymmetricKeyLifetime'));
$keyCredentials1->setMaxLifetime('P30D');
$keyCredentials1->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$keyCredentialsArray []= $keyCredentials1;
$applicationRestrictions->setKeyCredentials($keyCredentialsArray);

$result =  $graphClient->policies()->defaultAppManagementPolicy()->patch($requestRequestBody);


```