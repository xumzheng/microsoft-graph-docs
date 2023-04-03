---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = B2xIdentityUserFlow();
requestBody.setId('UserFlowWithAPIConnector');

requestBody.setUserFlowType(UserFlowType('signuporsignin'));

requestBody.setUserFlowTypeVersion(1);

apiConnectorConfiguration = UserFlowApiConnectorConfiguration();
apiConnectorConfigurationPostFederationSignup = IdentityApiConnector();
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostFederationSignup.setAdditionalData(additionalData);



apiConnectorConfiguration.setPostFederationSignup($apiConnectorConfigurationPostFederationSignup);
apiConnectorConfigurationPostAttributeCollection = IdentityApiConnector();
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostAttributeCollection.setAdditionalData(additionalData);



apiConnectorConfiguration.setPostAttributeCollection($apiConnectorConfigurationPostAttributeCollection);

requestBody.setApiConnectorConfiguration($apiConnectorConfiguration);


requestResult = graphServiceClient.identity().b2xUserFlows().post(requestBody);


```