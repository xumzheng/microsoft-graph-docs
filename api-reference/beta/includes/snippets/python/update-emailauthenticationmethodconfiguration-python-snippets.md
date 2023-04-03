---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthenticationMethodConfiguration();
requestBody.set@odatatype('#microsoft.graph.emailAuthenticationMethodConfiguration');

additionalData = [
'allowExternalIdToUseEmailOtp' => 'disabled', 
];
requestBody.setAdditionalData(additionalData);




result = await client.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(requestBody);


```