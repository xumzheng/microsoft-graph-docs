---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomAccessPackageWorkflowExtension()
request_body.displayName = 'test_action_0124'

request_body.description = 'this is for graph testing only'

endpointConfiguration = CustomExtensionEndpointConfiguration()
endpointConfiguration.@odatatype = '#microsoft.graph.logicAppTriggerEndpointConfiguration'

additionalData = [
'subscriptionId' => '38ab2ccc-3747-4567-b36b-9478f5602f0d', 
'resourceGroupName' => 'EMLogicApp', 
'logicAppWorkflowName' => 'customextension_test', 
];
endpointConfiguration.additionaldata(additionalData)



request_body.endpointConfiguration = endpointConfiguration
authenticationConfiguration = CustomExtensionAuthenticationConfiguration()
authenticationConfiguration.@odatatype = '#microsoft.graph.azureAdTokenAuthentication'

additionalData = [
'resourceId' => 'f604bd15-f785-4309-ad7c-6fad18ddb6cb', 
];
authenticationConfiguration.additionaldata(additionalData)



request_body.authenticationConfiguration = authenticationConfiguration



result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').customAccessPackageWorkflowExtensions.post(request_body = request_body)


```