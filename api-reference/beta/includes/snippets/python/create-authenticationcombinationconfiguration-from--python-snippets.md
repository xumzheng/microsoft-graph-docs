---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationCombinationConfiguration()
request_body.set@odatatype('#microsoft.graph.fido2CombinationConfiguration')

request_body.setAppliesToCombinations([request_body.setAuthenticationMethodModes(AuthenticationMethodModes('fido2'))
])

additionalData = [
'allowedAAGUIDs' => ['486c3b50-889c-480a-abc5-c04ef7c873e0', 'c042882f-a621-40c8-94d3-9cde3a826fed', 'ec454c08-4c77-4012-9d48-45f7f0fccdfb', ],
];
request_body.setAdditionalData(additionalData)




result = await client.identity.conditionalAccess.authenticationStrengths.policies._by_id('authenticationStrengthPolicy-id').combinationConfigurations.post(request_body)


```