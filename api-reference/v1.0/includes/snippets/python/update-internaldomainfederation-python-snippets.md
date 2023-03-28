---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InternalDomainFederation();
$requestBody->setDisplayName('Contoso name change');

$requestBody->setFederatedIdpMfaBehavior(new FederatedIdpMfaBehavior('acceptifmfadonebyfederatedidp'));



$requestResult = $graphServiceClient->domainsById('domain-id')->federationConfigurationById('internalDomainFederation-id')->patch($requestBody);


```