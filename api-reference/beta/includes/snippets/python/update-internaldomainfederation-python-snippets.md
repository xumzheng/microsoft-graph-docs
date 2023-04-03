---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = InternalDomainFederation();
requestBody.setDisplayName('Contoso name change');

requestBody.setFederatedIdpMfaBehavior(FederatedIdpMfaBehavior('acceptifmfadonebyfederatedidp'));



result = awaitclient.domainsById('domain-id').federationConfigurationById('internalDomainFederation-id').patch(requestBody);


```