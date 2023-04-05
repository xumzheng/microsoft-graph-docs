---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodConfiguration()
request_body.set@odatatype('#microsoft.graph.x509CertificateAuthenticationMethodConfiguration')

request_body.setId('X509Certificate')

request_body.setState(AuthenticationMethodState('enabled'))

additionalData = [
'certificateUserBindings' => certificateUserBindings1 = ()
		certificateUserBindings1.setX509CertificateField('PrincipalName')

		certificateUserBindings1.setUserProperty('onPremisesUserPrincipalName')

		certificateUserBindings1.setPriority(1)


certificateUserBindingsArray []= certificateUserBindings1;
request_body.setCertificateUserBindings(certificateUserBindingsArray)


'authenticationModeConfiguration' => request_body = AuthenticationModeConfiguration()
	request_body.setX509CertificateAuthenticationDefaultMode('x509CertificateMultiFactor')

rules1 = ()
	rules1.setX509CertificateRuleType('issuerSubject')

	rules1.setIdentifier('CN=ContosoCA,DC=Contoso,DC=org ')

	rules1.setX509CertificateAuthenticationMode('x509CertificateMultiFactor')


rulesArray []= rules1;
rules2 = ()
	rules2.setX509CertificateRuleType('policyOID')

	rules2.setIdentifier('1.2.3.4')

	rules2.setX509CertificateAuthenticationMode('x509CertificateMultiFactor')


rulesArray []= rules2;
request_body.setRules(rulesArray)



request_body.setAuthenticationModeConfiguration($authenticationModeConfiguration)

'includeTargets' => includeTargets1 = ()
includeTargets1.setTargetType('group')

includeTargets1.setId('all_users')

includeTargets1.setIsRegistrationRequired(false)


includeTargetsArray []= includeTargets1;
request_body.setIncludeTargets(includeTargetsArray)


];
request_body.setAdditionalData(additionalData)




result = await client.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsby_id('authenticationMethodConfiguration-id').patch(request_body)


```