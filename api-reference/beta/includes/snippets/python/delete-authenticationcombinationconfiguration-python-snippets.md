---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = AuthenticationCombinationConfigurationRequestBuilderDeleteRequestConfiguration(
)


await client.identity.conditionalAccess.authenticationStrengths.policies_by_id('authenticationStrengthPolicy-id').combinationConfigurations_by_id('authenticationCombinationConfiguration-id').delete()


```