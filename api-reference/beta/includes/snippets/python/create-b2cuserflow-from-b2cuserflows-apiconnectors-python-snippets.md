---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cIdentityUserFlow()
request_body.id = 'UserFlowWithAPIConnector'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.userFlowTypeVersion = 1

apiConnectorConfiguration = UserFlowApiConnectorConfiguration()
apiConnectorConfigurationPostFederationSignup = IdentityApiConnector()
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostFederationSignup.additionaldata(additionalData)



apiConnectorConfiguration.postFederationSignup = apiConnectorConfigurationPostFederationSignup
apiConnectorConfigurationPostAttributeCollection = IdentityApiConnector()
additionalData = [
'@odata.id' => '{apiConnectorId}', 
];
apiConnectorConfigurationPostAttributeCollection.additionaldata(additionalData)



apiConnectorConfiguration.postAttributeCollection = apiConnectorConfigurationPostAttributeCollection

request_body.apiConnectorConfiguration = apiConnectorConfiguration


request_configuration = B2cUserFlowsRequestBuilderPostRequestConfiguration(
)


result = await client.identity.b2cUserFlows.post(request_body = request_body)


```