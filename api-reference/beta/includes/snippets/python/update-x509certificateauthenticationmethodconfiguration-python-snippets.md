---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.@odatatype = '#microsoft.graph.x509CertificateAuthenticationMethodConfiguration'

request_body.id = 'X509Certificate'

request_body.State(AuthenticationMethodState('enabled'))

additionalData = [
'certificateUserBindings' => certificateUserBindings1 = ()
		certificateUserBindings1.x509CertificateField = 'PrincipalName'

		certificateUserBindings1.userProperty = 'onPremisesUserPrincipalName'

		certificateUserBindings1.priority = 1


certificateUserBindingsArray []= certificateUserBindings1;
request_body.certificateuserbindings(certificateUserBindingsArray)


'authenticationModeConfiguration' => request_body = AuthenticationModeConfiguration()
	request_body.x509CertificateAuthenticationDefaultMode = 'x509CertificateMultiFactor'

rules1 = ()
	rules1.x509CertificateRuleType = 'issuerSubject'

	rules1.identifier = 'CN=ContosoCA,DC=Contoso,DC=org '

	rules1.x509CertificateAuthenticationMode = 'x509CertificateMultiFactor'


rulesArray []= rules1;
rules2 = ()
	rules2.x509CertificateRuleType = 'policyOID'

	rules2.identifier = '1.2.3.4'

	rules2.x509CertificateAuthenticationMode = 'x509CertificateMultiFactor'


rulesArray []= rules2;
request_body.rules(rulesArray)



request_body.authenticationModeConfiguration = authenticationModeConfiguration

'includeTargets' => includeTargets1 = ()
includeTargets1.targetType = 'group'

includeTargets1.id = 'all_users'

includeTargets1.isRegistrationRequired = false


includeTargetsArray []= includeTargets1;
request_body.includetargets(includeTargetsArray)


];
request_body.additionaldata(additionalData)




request_configuration = AuthenticationMethodConfigurationRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurations_by_id('authenticationMethodConfiguration-id').patch(request_body = request_body)


```