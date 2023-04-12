---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TenantAppManagementPolicy()
request_body.isEnabled = true

applicationRestrictions = AppManagementConfiguration()
passwordCredentialsPasswordCredentialConfiguration1 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration1.RestrictionType(AppCredentialRestrictionType('passwordaddition'))

passwordCredentialsPasswordCredentialConfiguration1.maxLifetime=null

passwordCredentialsPasswordCredentialConfiguration1.restrictForAppsCreatedAfterDateTime = DateTime('2021-01-01T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration1;
passwordCredentialsPasswordCredentialConfiguration2 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration2.RestrictionType(AppCredentialRestrictionType('passwordlifetime'))

passwordCredentialsPasswordCredentialConfiguration2.maxlifetime =  \DateInterval('P4DT12H30M5S')

passwordCredentialsPasswordCredentialConfiguration2.restrictForAppsCreatedAfterDateTime = DateTime('2017-01-01T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration2;
passwordCredentialsPasswordCredentialConfiguration3 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration3.RestrictionType(AppCredentialRestrictionType('symmetrickeyaddition'))

passwordCredentialsPasswordCredentialConfiguration3.maxLifetime=null

passwordCredentialsPasswordCredentialConfiguration3.restrictForAppsCreatedAfterDateTime = DateTime('2021-01-01T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration3;
passwordCredentialsPasswordCredentialConfiguration4 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration4.RestrictionType(AppCredentialRestrictionType('custompasswordaddition'))

passwordCredentialsPasswordCredentialConfiguration4.maxLifetime=null

passwordCredentialsPasswordCredentialConfiguration4.restrictForAppsCreatedAfterDateTime = DateTime('2015-01-01T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration4;
passwordCredentialsPasswordCredentialConfiguration5 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration5.RestrictionType(AppCredentialRestrictionType('symmetrickeylifetime'))

passwordCredentialsPasswordCredentialConfiguration5.maxlifetime =  \DateInterval('P40D')

passwordCredentialsPasswordCredentialConfiguration5.restrictForAppsCreatedAfterDateTime = DateTime('2015-01-01T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration5;
applicationRestrictions.passwordcredentials(passwordCredentialsArray)


keyCredentialsKeyCredentialConfiguration1 = KeyCredentialConfiguration()
keyCredentialsKeyCredentialConfiguration1.RestrictionType(AppKeyCredentialRestrictionType('asymmetrickeylifetime'))

keyCredentialsKeyCredentialConfiguration1.maxlifetime =  \DateInterval('P30D')

keyCredentialsKeyCredentialConfiguration1.restrictForAppsCreatedAfterDateTime = DateTime('2015-01-01T10:37:00Z')


keyCredentialsArray []= keyCredentialsKeyCredentialConfiguration1;
applicationRestrictions.keycredentials(keyCredentialsArray)



request_body.applicationRestrictions = applicationRestrictions



result = await client.policies.defaultAppManagementPolicy.patch(request_body = request_body)


```