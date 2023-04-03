---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = B2xIdentityUserFlow();
requestBody.setId('UserFlowWithAPIConnector');

requestBody.setUserFlowType(UserFlowType('signuporsignin'));

requestBody.setUserFlowTypeVersion(1);

apiConnectorConfiguration = UserFlowApiConnectorConfiguration();
apiConnectorConfigurationPostFederationSignup = IdentityApiConnector();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}', 
];
apiConnectorConfigurationPostFederationSignup.setAdditionalData(additionalData);



apiConnectorConfiguration.setPostFederationSignup($apiConnectorConfigurationPostFederationSignup);
apiConnectorConfigurationPostAttributeCollection = IdentityApiConnector();
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}', 
];
apiConnectorConfigurationPostAttributeCollection.setAdditionalData(additionalData);



apiConnectorConfiguration.setPostAttributeCollection($apiConnectorConfigurationPostAttributeCollection);

requestBody.setApiConnectorConfiguration($apiConnectorConfiguration);


result = await client.identity().b2xUserFlows().post(requestBody);


```