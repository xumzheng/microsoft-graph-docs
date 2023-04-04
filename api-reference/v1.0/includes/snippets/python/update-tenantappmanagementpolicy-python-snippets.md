---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = TenantAppManagementPolicy();
request_body.setIsEnabled(true);

applicationRestrictions = AppManagementConfiguration();
passwordCredentialsPasswordCredentialConfiguration1 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration1.setRestrictionType(AppCredentialRestrictionType('passwordaddition'));

passwordCredentialsPasswordCredentialConfiguration1.setMaxLifetime(null);

passwordCredentialsPasswordCredentialConfiguration1.setRestrictForAppsCreatedAfterDateTime(DateTime('2021-01-01T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration1;
passwordCredentialsPasswordCredentialConfiguration2 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration2.setRestrictionType(AppCredentialRestrictionType('passwordlifetime'));

$passwordCredentialsPasswordCredentialConfiguration2.setMaxLifetime( \DateInterval('P4DT12H30M5S'));

passwordCredentialsPasswordCredentialConfiguration2.setRestrictForAppsCreatedAfterDateTime(DateTime('2017-01-01T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration2;
passwordCredentialsPasswordCredentialConfiguration3 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration3.setRestrictionType(AppCredentialRestrictionType('symmetrickeyaddition'));

passwordCredentialsPasswordCredentialConfiguration3.setMaxLifetime(null);

passwordCredentialsPasswordCredentialConfiguration3.setRestrictForAppsCreatedAfterDateTime(DateTime('2021-01-01T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration3;
passwordCredentialsPasswordCredentialConfiguration4 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration4.setRestrictionType(AppCredentialRestrictionType('custompasswordaddition'));

passwordCredentialsPasswordCredentialConfiguration4.setMaxLifetime(null);

passwordCredentialsPasswordCredentialConfiguration4.setRestrictForAppsCreatedAfterDateTime(DateTime('2015-01-01T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration4;
passwordCredentialsPasswordCredentialConfiguration5 = PasswordCredentialConfiguration();
passwordCredentialsPasswordCredentialConfiguration5.setRestrictionType(AppCredentialRestrictionType('symmetrickeylifetime'));

$passwordCredentialsPasswordCredentialConfiguration5.setMaxLifetime( \DateInterval('P40D'));

passwordCredentialsPasswordCredentialConfiguration5.setRestrictForAppsCreatedAfterDateTime(DateTime('2015-01-01T10:37:00Z'));


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration5;
applicationRestrictions.setPasswordCredentials(passwordCredentialsArray);


keyCredentialsKeyCredentialConfiguration1 = KeyCredentialConfiguration();
keyCredentialsKeyCredentialConfiguration1.setRestrictionType(AppKeyCredentialRestrictionType('asymmetrickeylifetime'));

$keyCredentialsKeyCredentialConfiguration1.setMaxLifetime( \DateInterval('P30D'));

keyCredentialsKeyCredentialConfiguration1.setRestrictForAppsCreatedAfterDateTime(DateTime('2015-01-01T10:37:00Z'));


keyCredentialsArray []= keyCredentialsKeyCredentialConfiguration1;
applicationRestrictions.setKeyCredentials(keyCredentialsArray);



request_body.setApplicationRestrictions($applicationRestrictions);


result = await client.policies.defaultAppManagementPolicy.patch(request_body);


```