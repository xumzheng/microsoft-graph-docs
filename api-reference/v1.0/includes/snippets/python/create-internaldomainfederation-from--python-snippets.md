---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InternalDomainFederation()
request_body.@odatatype = '#microsoft.graph.internalDomainFederation'

request_body.displayName = 'Contoso'

request_body.issuerUri = 'http://contoso.com/adfs/services/trust'

request_body.metadataExchangeUri = 'https://sts.contoso.com/adfs/services/trust/mex'

request_body.signingCertificate = 'MIIE3jCCAsagAwIBAgIQQcyDaZz3MI'

request_body.passiveSignInUri = 'https://sts.contoso.com/adfs/ls'

request_body.PreferredAuthenticationProtocol(AuthenticationProtocol('wsfed'))

request_body.activeSignInUri = 'https://sts.contoso.com/adfs/services/trust/2005/usernamemixed'

request_body.signOutUri = 'https://sts.contoso.com/adfs/ls'

request_body.PromptLoginBehavior(PromptLoginBehavior('nativesupport'))

request_body.is_signed_authentication_request_required = True

request_body.nextSigningCertificate = 'MIIE3jCCAsagAwIBAgIQQcyDaZz3MI'

request_body.FederatedIdpMfaBehavior(FederatedIdpMfaBehavior('rejectmfabyfederatedidp'))




result = await client.domains_by_id('domain-id').federationConfiguration.post(request_body = request_body)


```