---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomCalloutExtension()
additionalData = [
'value' => request_body = Value()
		request_body.set@odatatype('#microsoft.graph.accessPackageAssignmentRequestWorkflowExtension')

		request_body.setDisplayName('test_action_0124_email')

		request_body.setDescription('this is for graph testing only')

endpointConfiguration = EndpointConfiguration()
		endpointConfiguration.set@odatatype('#microsoft.graph.logicAppTriggerEndpointConfiguration')

		endpointConfiguration.setSubscriptionId('38ab2ccc-3747-4567-b36b-9478f5602f0d')

		endpointConfiguration.setResourceGroupName('test')

		endpointConfiguration.setLogicAppWorkflowName('elm-extension-email')


request_body.setEndpointConfiguration($endpointConfiguration)
authenticationConfiguration = AuthenticationConfiguration()
		authenticationConfiguration.set@odatatype('#microsoft.graph.azureAdPopTokenAuthentication')


request_body.setAuthenticationConfiguration($authenticationConfiguration)
callbackConfiguration = CallbackConfiguration()
		callbackConfiguration.set@odatatype('microsoft.graph.customExtensionCallbackConfiguration')

		callbackConfiguration.setDurationBeforeTimeout('PT1H')


request_body.setCallbackConfiguration($callbackConfiguration)

request_body.setValue($value)

];
request_body.setAdditionalData(additionalData)




result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs._by_id('accessPackageCatalog-id').accessPackageCustomWorkflowExtensions.post(request_body)


```