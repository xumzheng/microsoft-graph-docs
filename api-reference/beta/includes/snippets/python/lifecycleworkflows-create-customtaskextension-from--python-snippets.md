---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomTaskExtension();
requestBody.setDisplayName('Grant manager access to mailbox and OneDrive');

requestBody.setDescription('Grant manager access to mailbox and OneDrive');

endpointConfiguration = CustomExtensionEndpointConfiguration();
endpointConfiguration.set@odatatype('#microsoft.graph.logicAppTriggerEndpointConfiguration');

additionalData = [
'subscriptionId' => 'c500b67c-e9b7-4ad2-a90d-77d41385ae55', 
'resourceGroupName' => 'RG-LCM', 
'logicAppWorkflowName' => 'ManagerAccess', 
];
endpointConfiguration.setAdditionalData(additionalData);



requestBody.setEndpointConfiguration($endpointConfiguration);
authenticationConfiguration = CustomExtensionAuthenticationConfiguration();
authenticationConfiguration.set@odatatype('#microsoft.graph.azureAdTokenAuthentication');

additionalData = [
'resourceId' => '542dc01a-0b5d-4edc-b3f9-5cfe6393f557', 
];
authenticationConfiguration.setAdditionalData(additionalData);



requestBody.setAuthenticationConfiguration($authenticationConfiguration);
clientConfiguration = CustomExtensionClientConfiguration();
clientConfiguration.set@odatatype('#microsoft.graph.customExtensionClientConfiguration');

clientConfiguration.setTimeoutInMilliseconds(1000);

additionalData = [
'maximumRetries' => 1,
];
clientConfiguration.setAdditionalData(additionalData);



requestBody.setClientConfiguration($clientConfiguration);
callbackConfiguration = CustomExtensionCallbackConfiguration();
callbackConfiguration.set@odatatype('#microsoft.graph.identityGovernance.customTaskExtensionCallbackConfiguration');

$callbackConfiguration.setTimeoutDuration( \DateInterval('PT5M'));


requestBody.setCallbackConfiguration($callbackConfiguration);


result = await client.identityGovernance().lifecycleWorkflows().customTaskExtensions().post(requestBody);


```