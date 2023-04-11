---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomCalloutExtension()
additionalData = [
'value' => request_body = Value()
		request_body.@odatatype = '#microsoft.graph.accessPackageAssignmentRequestWorkflowExtension'

		request_body.displayName = 'test_action_0124_email'

		request_body.description = 'this is for graph testing only'

endpointConfiguration = EndpointConfiguration()
		endpointConfiguration.@odatatype = '#microsoft.graph.logicAppTriggerEndpointConfiguration'

		endpointConfiguration.subscriptionId = '38ab2ccc-3747-4567-b36b-9478f5602f0d'

		endpointConfiguration.resourceGroupName = 'test'

		endpointConfiguration.logicAppWorkflowName = 'elm-extension-email'


request_body.endpointConfiguration = endpointConfiguration
authenticationConfiguration = AuthenticationConfiguration()
		authenticationConfiguration.@odatatype = '#microsoft.graph.azureAdPopTokenAuthentication'


request_body.authenticationConfiguration = authenticationConfiguration
callbackConfiguration = CallbackConfiguration()
		callbackConfiguration.@odatatype = 'microsoft.graph.customExtensionCallbackConfiguration'

		callbackConfiguration.durationBeforeTimeout = 'PT1H'


request_body.callbackConfiguration = callbackConfiguration

request_body.value = value

];
request_body.additionaldata(additionalData)




request_configuration = AccessPackageCustomWorkflowExtensionsRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageCustomWorkflowExtensions.post(request_body = request_body)


```