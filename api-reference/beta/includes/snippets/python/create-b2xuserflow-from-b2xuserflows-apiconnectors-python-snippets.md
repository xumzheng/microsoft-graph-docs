---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2xIdentityUserFlow()
request_body.setId('UserFlowWithAPIConnector')

request_body.setUserFlowType(UserFlowType('signuporsignin'))

request_body.setUserFlowTypeVersion(1)

apiConnectorConfiguration = UserFlowApiConnectorConfiguration()
apiConnectorConfigurationPostFederationSignup = IdentityApiConnector()
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostFederationSignup.setAdditionalData(additionalData)



apiConnectorConfiguration.setPostFederationSignup($apiConnectorConfigurationPostFederationSignup)
apiConnectorConfigurationPostAttributeCollection = IdentityApiConnector()
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostAttributeCollection.setAdditionalData(additionalData)



apiConnectorConfiguration.setPostAttributeCollection($apiConnectorConfigurationPostAttributeCollection)

request_body.setApiConnectorConfiguration($apiConnectorConfiguration)


result = await client.identity.b2xUserFlows.post(request_body, headers=)


```