---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AppManagementPolicie()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}', 
];
request_body.setAdditionalData(additionalData)



request_config = AppManagementPolicyRequestBuilderPostRequestConfiguration(
request_config = AppManagementPolicyRequestBuilderPostRequestConfiguration(query_params=)


await client.servicePrincipals_by_id('servicePrincipal-id').appManagementPolicies_by_id('appManagementPolicy-id').post(request_body, headers=)


```