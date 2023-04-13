---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicy()
request_body.displayName = 'Credential management policy'

request_body.description = 'Cred policy sample'

request_body.isEnabled = true

restrictions = AppManagementConfiguration()
passwordCredentialsPasswordCredentialConfiguration1 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration1.RestrictionType(AppCredentialRestrictionType('passwordaddition'))

passwordCredentialsPasswordCredentialConfiguration1.maxLifetime=null

passwordCredentialsPasswordCredentialConfiguration1.restrictForAppsCreatedAfterDateTime = DateTime('2019-10-19T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration1;
passwordCredentialsPasswordCredentialConfiguration2 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration2.RestrictionType(AppCredentialRestrictionType('passwordlifetime'))

passwordCredentialsPasswordCredentialConfiguration2.maxlifetime =  \DateInterval('P4DT12H30M5S')

passwordCredentialsPasswordCredentialConfiguration2.restrictForAppsCreatedAfterDateTime = DateTime('2014-10-19T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration2;
passwordCredentialsPasswordCredentialConfiguration3 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration3.RestrictionType(AppCredentialRestrictionType('symmetrickeyaddition'))

passwordCredentialsPasswordCredentialConfiguration3.maxLifetime=null

passwordCredentialsPasswordCredentialConfiguration3.restrictForAppsCreatedAfterDateTime = DateTime('2019-10-19T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration3;
passwordCredentialsPasswordCredentialConfiguration4 = PasswordCredentialConfiguration()
passwordCredentialsPasswordCredentialConfiguration4.RestrictionType(AppCredentialRestrictionType('symmetrickeylifetime'))

passwordCredentialsPasswordCredentialConfiguration4.maxlifetime =  \DateInterval('P4D')

passwordCredentialsPasswordCredentialConfiguration4.restrictForAppsCreatedAfterDateTime = DateTime('2014-10-19T10:37:00Z')


passwordCredentialsArray []= passwordCredentialsPasswordCredentialConfiguration4;
restrictions.passwordcredentials(passwordCredentialsArray)


keyCredentialsKeyCredentialConfiguration1 = KeyCredentialConfiguration()
keyCredentialsKeyCredentialConfiguration1.RestrictionType(AppKeyCredentialRestrictionType('asymmetrickeylifetime'))

keyCredentialsKeyCredentialConfiguration1.maxlifetime =  \DateInterval('P90D')

keyCredentialsKeyCredentialConfiguration1.restrictForAppsCreatedAfterDateTime = DateTime('2014-10-19T10:37:00Z')


keyCredentialsArray []= keyCredentialsKeyCredentialConfiguration1;
restrictions.keycredentials(keyCredentialsArray)



request_body.restrictions = restrictions



result = await client.policies.appManagementPolicies.post(request_body = request_body)


```