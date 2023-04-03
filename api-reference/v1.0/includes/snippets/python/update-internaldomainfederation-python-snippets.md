---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = InternalDomainFederation();
requestBody.setDisplayName('Contoso name change');

requestBody.setFederatedIdpMfaBehavior(FederatedIdpMfaBehavior('acceptifmfadonebyfederatedidp'));



result = await client.domainsById('domain-id').federationConfigurationById('internalDomainFederation-id').patch(requestBody);


```