---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InternalDomainFederation()
request_body.set@odatatype('#microsoft.graph.internalDomainFederation')

request_body.setDisplayName('Contoso')

request_body.setIssuerUri('http://contoso.com/adfs/services/trust')

request_body.setMetadataExchangeUri('https://sts.contoso.com/adfs/services/trust/mex')

request_body.setSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI')

request_body.setPassiveSignInUri('https://sts.contoso.com/adfs/ls')

request_body.setPreferredAuthenticationProtocol(AuthenticationProtocol('wsfed'))

request_body.setActiveSignInUri('https://sts.contoso.com/adfs/services/trust/2005/usernamemixed')

request_body.setSignOutUri('https://sts.contoso.com/adfs/ls')

request_body.setPromptLoginBehavior(PromptLoginBehavior('nativesupport'))

request_body.setIsSignedAuthenticationRequestRequired(true)

request_body.setNextSigningCertificate('MIIE3jCCAsagAwIBAgIQQcyDaZz3MI')

request_body.setFederatedIdpMfaBehavior(FederatedIdpMfaBehavior('rejectmfabyfederatedidp'))


request_config = FederationConfigurationRequestBuilderPostRequestConfiguration(
request_config = FederationConfigurationRequestBuilderPostRequestConfiguration(query_params=)


result = await client.domains_by_id('domain-id').federationConfiguration.post(request_body, headers=)


```