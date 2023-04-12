---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomTaskExtension()
request_body.displayName = 'Grant manager access to mailbox and OneDrive'

request_body.description = 'Grant manager access to mailbox and OneDrive'

endpointConfiguration = CustomExtensionEndpointConfiguration()
endpointConfiguration.@odatatype = '#microsoft.graph.logicAppTriggerEndpointConfiguration'

additionalData = [
'subscriptionId' => 'c500b67c-e9b7-4ad2-a90d-77d41385ae55', 
'resourceGroupName' => 'RG-LCM', 
'logicAppWorkflowName' => 'ManagerAccess', 
];
endpointConfiguration.additionaldata(additionalData)



request_body.endpointConfiguration = endpointConfiguration
authenticationConfiguration = CustomExtensionAuthenticationConfiguration()
authenticationConfiguration.@odatatype = '#microsoft.graph.azureAdTokenAuthentication'

additionalData = [
'resourceId' => '542dc01a-0b5d-4edc-b3f9-5cfe6393f557', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration
clientConfiguration = CustomExtensionClientConfiguration()
clientConfiguration.@odatatype = '#microsoft.graph.customExtensionClientConfiguration'

clientConfiguration.timeoutInMilliseconds = 1000

additionalData = [
'maximumRetries' => 1,
];
clientConfiguration.additionaldata(additionalData)



request_body.clientConfiguration = clientConfiguration
callbackConfiguration = CustomExtensionCallbackConfiguration()
callbackConfiguration.@odatatype = '#microsoft.graph.identityGovernance.customTaskExtensionCallbackConfiguration'

callbackConfiguration.timeoutduration =  \DateInterval('PT20M')


request_body.callbackConfiguration = callbackConfiguration



result = await client.identityGovernance.lifecycleWorkflows.customTaskExtensions_by_id('customTaskExtension-id').patch(request_body = request_body)


```