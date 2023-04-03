---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CustomCalloutExtension();
additionalData = [
'value' => requestBody = Value();
		requestBody.set@odatatype('#microsoft.graph.accessPackageAssignmentRequestWorkflowExtension');

		requestBody.setDisplayName('test_action_0124_email');

		requestBody.setDescription('this is for graph testing only');

endpointConfiguration = EndpointConfiguration();
		endpointConfiguration.set@odatatype('#microsoft.graph.logicAppTriggerEndpointConfiguration');

		endpointConfiguration.setSubscriptionId('38ab2ccc-3747-4567-b36b-9478f5602f0d');

		endpointConfiguration.setResourceGroupName('test');

		endpointConfiguration.setLogicAppWorkflowName('elm-extension-email');


requestBody.setEndpointConfiguration($endpointConfiguration);
authenticationConfiguration = AuthenticationConfiguration();
		authenticationConfiguration.set@odatatype('#microsoft.graph.azureAdPopTokenAuthentication');


requestBody.setAuthenticationConfiguration($authenticationConfiguration);
callbackConfiguration = CallbackConfiguration();
		callbackConfiguration.set@odatatype('microsoft.graph.customExtensionCallbackConfiguration');

		callbackConfiguration.setDurationBeforeTimeout('PT1H');


requestBody.setCallbackConfiguration($callbackConfiguration);

requestBody.setValue($value);

];
requestBody.setAdditionalData(additionalData);




result = await client.identityGovernance().entitlementManagement().accessPackageCatalogsById('accessPackageCatalog-id').accessPackageCustomWorkflowExtensions().post(requestBody);


```