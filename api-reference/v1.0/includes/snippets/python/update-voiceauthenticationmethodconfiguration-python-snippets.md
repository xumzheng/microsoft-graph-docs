---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationMethodConfiguration();
requestBody.set@odatatype('#microsoft.graph.voiceAuthenticationMethodConfiguration');

additionalData = [
'isOfficePhoneAllowed' => 'false', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurationsById('authenticationMethodConfiguration-id').patch(requestBody);


```