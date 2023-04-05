---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomAccessPackageWorkflowExtension()
request_body.setDisplayName('test_action_0124')

request_body.setDescription('this is for graph testing only')

endpointConfiguration = CustomExtensionEndpointConfiguration()
endpointConfiguration.set@odatatype('#microsoft.graph.logicAppTriggerEndpointConfiguration')

additionalData = [
'subscriptionId' => '38ab2ccc-3747-4567-b36b-9478f5602f0d', 
'resourceGroupName' => 'EMLogicApp', 
'logicAppWorkflowName' => 'customextension_test', 
];
endpointConfiguration.setAdditionalData(additionalData)



request_body.setEndpointConfiguration($endpointConfiguration)
authenticationConfiguration = CustomExtensionAuthenticationConfiguration()
authenticationConfiguration.set@odatatype('#microsoft.graph.azureAdTokenAuthentication')

additionalData = [
'resourceId' => 'f604bd15-f785-4309-ad7c-6fad18ddb6cb', 
];
authenticationConfiguration.setAdditionalData(additionalData)



request_body.setAuthenticationConfiguration($authenticationConfiguration)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogsby_id('accessPackageCatalog-id').customAccessPackageWorkflowExtensions.post(request_body)


```