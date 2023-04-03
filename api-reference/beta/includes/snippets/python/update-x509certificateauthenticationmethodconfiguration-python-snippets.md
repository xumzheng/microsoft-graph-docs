---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthenticationMethodConfiguration();
requestBody.set@odatatype('#microsoft.graph.x509CertificateAuthenticationMethodConfiguration');

requestBody.setId('X509Certificate');

requestBody.setState(AuthenticationMethodState('enabled'));

additionalData = [
'certificateUserBindings' => certificateUserBindings1 = ();
		certificateUserBindings1.setX509CertificateField('PrincipalName');

		certificateUserBindings1.setUserProperty('onPremisesUserPrincipalName');

		certificateUserBindings1.setPriority(1);


certificateUserBindingsArray []= certificateUserBindings1;
requestBody.setCertificateUserBindings(certificateUserBindingsArray);


'authenticationModeConfiguration' => requestBody = AuthenticationModeConfiguration();
	requestBody.setX509CertificateAuthenticationDefaultMode('x509CertificateMultiFactor');

rules1 = ();
	rules1.setX509CertificateRuleType('issuerSubject');

	rules1.setIdentifier('CN=ContosoCA,DC=Contoso,DC=org ');

	rules1.setX509CertificateAuthenticationMode('x509CertificateMultiFactor');


rulesArray []= rules1;
rules2 = ();
	rules2.setX509CertificateRuleType('policyOID');

	rules2.setIdentifier('1.2.3.4');

	rules2.setX509CertificateAuthenticationMode('x509CertificateMultiFactor');


rulesArray []= rules2;
requestBody.setRules(rulesArray);



requestBody.setAuthenticationModeConfiguration($authenticationModeConfiguration);

'includeTargets' => includeTargets1 = ();
includeTargets1.setTargetType('group');

includeTargets1.setId('all_users');

includeTargets1.setIsRegistrationRequired(false);


includeTargetsArray []= includeTargets1;
requestBody.setIncludeTargets(includeTargetsArray);


];
requestBody.setAdditionalData(additionalData);




result = await client.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(requestBody);


```