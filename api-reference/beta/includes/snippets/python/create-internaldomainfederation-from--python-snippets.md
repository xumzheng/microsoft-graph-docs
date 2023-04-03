---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = InternalDomainFederation();
requestBody.set@odatatype('#microsoft.graph.internalDomainFederation');

requestBody.setDisplayName('Contoso');

requestBody.setIssuerUri('http://contoso.com/adfs/services/trust');

requestBody.setMetadataExchangeUri('https://sts.contoso.com/adfs/services/trust/mex');

requestBody.setSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI');

requestBody.setPassiveSignInUri('https://sts.contoso.com/adfs/ls');

requestBody.setPreferredAuthenticationProtocol(AuthenticationProtocol('wsfed'));

requestBody.setActiveSignInUri('https://sts.contoso.com/adfs/services/trust/2005/usernamemixed');

requestBody.setSignOutUri('https://sts.contoso.com/adfs/ls');

requestBody.setPromptLoginBehavior(PromptLoginBehavior('nativesupport'));

requestBody.setIsSignedAuthenticationRequestRequired(true);

requestBody.setNextSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI');

requestBody.setFederatedIdpMfaBehavior(FederatedIdpMfaBehavior('rejectmfabyfederatedidp'));



result = await client.domainsById('domain-id').federationConfiguration().post(requestBody);


```