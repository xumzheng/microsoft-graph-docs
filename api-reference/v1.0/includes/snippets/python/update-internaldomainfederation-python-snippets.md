---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InternalDomainFederation()
request_body.setDisplayName('Contoso name change')

request_body.setFederatedIdpMfaBehavior(FederatedIdpMfaBehavior('acceptifmfadonebyfederatedidp'))



result = await client.domains._by_id('domain-id').federationConfiguration._by_id('internalDomainFederation-id').patch(request_body)


```