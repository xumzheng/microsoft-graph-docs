---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IdentityApiConnector();
$requestBody.setDisplayName('Test API');

$requestBody.setTargetUrl('https://someapi.com/api');

$authenticationConfiguration = new ApiAuthenticationConfigurationBase();
$authenticationConfiguration.set@odatatype('#microsoft.graph.basicAuthentication');

$additionalData = [
'username' => 'MyUsername', 
'password' => 'MyPassword', 
];
$authenticationConfiguration.setAdditionalData($additionalData);



$requestBody.setAuthenticationConfiguration($authenticationConfiguration);


$requestResult = $graphServiceClient.identity().apiConnectors().post($requestBody);


```