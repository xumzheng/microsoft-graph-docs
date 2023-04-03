---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AppManagementPolicy();
requestBody.setDisplayName('Credential management policy');

requestBody.setDescription('Cred policy sample');

requestBody.setIsEnabled(true);

restrictions = AppManagementConfiguration();
passwordCredentialsPasswordCredentialConfiguration1 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration1.setRestrictionType(AppCredentialRestrictionType('passwordaddition'));

passwordCredentialsPasswordCredentialConfiguration1.setMaxLifetime(null);

passwordCredentialsPasswordCredentialConfiguration1.setRestrictForAppsCreatedAfterDateTime(DateTime('2019-10-19T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration1;
passwordCredentialsPasswordCredentialConfiguration2 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration2.setRestrictionType(AppCredentialRestrictionType('passwordlifetime'));

$passwordCredentialsPasswordCredentialConfiguration2.setMaxLifetime( \DateInterval('P4DT12H30M5S'));

passwordCredentialsPasswordCredentialConfiguration2.setRestrictForAppsCreatedAfterDateTime(DateTime('2014-10-19T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration2;
passwordCredentialsPasswordCredentialConfiguration3 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration3.setRestrictionType(AppCredentialRestrictionType('symmetrickeyaddition'));

passwordCredentialsPasswordCredentialConfiguration3.setMaxLifetime(null);

passwordCredentialsPasswordCredentialConfiguration3.setRestrictForAppsCreatedAfterDateTime(DateTime('2019-10-19T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration3;
passwordCredentialsPasswordCredentialConfiguration4 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration4.setRestrictionType(AppCredentialRestrictionType('symmetrickeylifetime'));

$passwordCredentialsPasswordCredentialConfiguration4.setMaxLifetime( \DateInterval('P4D'));

passwordCredentialsPasswordCredentialConfiguration4.setRestrictForAppsCreatedAfterDateTime(DateTime('2014-10-19T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration4;
restrictions.setPasswordCredentials(passwordCredentialsArray);


keyCredentialsKeyCredentialConfiguration1 = KeyCredentialConfiguration();
keyCredentialsKeyCredentialConfiguration1.setRestrictionType(AppKeyCredentialRestrictionType('asymmetrickeylifetime'));

$keyCredentialsKeyCredentialConfiguration1.setMaxLifetime( \DateInterval('P90D'));

keyCredentialsKeyCredentialConfiguration1.setRestrictForAppsCreatedAfterDateTime(DateTime('2014-10-19T10:37:00Z'));


keyCredentialsArray []= keyCredentialsKeyCredentialConfiguration1;
restrictions.setKeyCredentials(keyCredentialsArray);



requestBody.setRestrictions($restrictions);


result = awaitclient.policies().appManagementPolicies().post(requestBody);


```