---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustomCalloutExtension()
additionalData = [
'value' => request_body = Value()
		request_body.@odatatype = '#microsoft.graph.accessPackageAssignmentWorkflowExtension'

		request_body.displayName = 'test_action_0127_email'

		request_body.description = 'this is for graph testing only'

endpoint_configuration = EndpointConfiguration()
		endpointConfiguration.@odatatype = '#microsoft.graph.logicAppTriggerEndpointConfiguration'

		endpointConfiguration.subscriptionId = '38ab2ccc-3747-4567-b36b-9478f5602f0d'

		endpointConfiguration.resourceGroupName = 'test'

		endpointConfiguration.logicAppWorkflowName = 'elm-extension-email'


request_body.endpoint_configuration = endpointConfiguration
authentication_configuration = AuthenticationConfiguration()
		authenticationConfiguration.@odatatype = '#microsoft.graph.azureAdPopTokenAuthentication'


request_body.authentication_configuration = authenticationConfiguration

request_body.value = value

];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.entitlementManagement.accessPackageCatalogs_by_id('accessPackageCatalog-id').accessPackageCustomWorkflowExtensions.post(request_body = request_body)


```