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

$passwordCredentialspasswordCredentials1 = new PasswordCredentialConfiguration();

$passwordCredentialspasswordCredentials1->setRestrictionType(new AppCredentialRestrictionType('passwordAddition'));
$passwordCredentialspasswordCredentials1->setMaxLifetime(null);
$passwordCredentialspasswordCredentials1->setRestrictForAppsCreatedAfterDateTime(new DateTime("2021-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentialspasswordCredentials1;

$passwordCredentialspasswordCredentials2 = new PasswordCredentialConfiguration();

$passwordCredentialspasswordCredentials2->setRestrictionType(new AppCredentialRestrictionType('passwordLifetime'));
$passwordCredentialspasswordCredentials2->setMaxLifetime('P4DT12H30M5S');
$passwordCredentialspasswordCredentials2->setRestrictForAppsCreatedAfterDateTime(new DateTime("2017-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentialspasswordCredentials2;

$passwordCredentialspasswordCredentials3 = new PasswordCredentialConfiguration();

$passwordCredentialspasswordCredentials3->setRestrictionType(new AppCredentialRestrictionType('symmetricKeyAddition'));
$passwordCredentialspasswordCredentials3->setMaxLifetime(null);
$passwordCredentialspasswordCredentials3->setRestrictForAppsCreatedAfterDateTime(new DateTime("2021-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentialspasswordCredentials3;

$passwordCredentialspasswordCredentials4 = new PasswordCredentialConfiguration();

$passwordCredentialspasswordCredentials4->setRestrictionType(new AppCredentialRestrictionType('customPasswordAddition'));
$passwordCredentialspasswordCredentials4->setMaxLifetime(null);
$passwordCredentialspasswordCredentials4->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentialspasswordCredentials4;

$passwordCredentialspasswordCredentials5 = new PasswordCredentialConfiguration();

$passwordCredentialspasswordCredentials5->setRestrictionType(new AppCredentialRestrictionType('symmetricKeyLifetime'));
$passwordCredentialspasswordCredentials5->setMaxLifetime('P40D');
$passwordCredentialspasswordCredentials5->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$passwordCredentialsArray []= $passwordCredentialspasswordCredentials5;
$applicationRestrictions->setPasswordCredentials($passwordCredentialsArray);
$keyCredentialsArray = [];

$keyCredentialskeyCredentials1 = new KeyCredentialConfiguration();

$keyCredentialskeyCredentials1->setRestrictionType(new AppKeyCredentialRestrictionType('asymmetricKeyLifetime'));
$keyCredentialskeyCredentials1->setMaxLifetime('P30D');
$keyCredentialskeyCredentials1->setRestrictForAppsCreatedAfterDateTime(new DateTime("2015-01-01T10:37:00Z"));

$keyCredentialsArray []= $keyCredentialskeyCredentials1;
$applicationRestrictions->setKeyCredentials($keyCredentialsArray);

$result =  $graphClient->policies()->defaultAppManagementPolicy()->patch($requestRequestBody);


```