---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2xIdentityUserFlow()
request_body.id = 'UserFlowWithAPIConnector'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.user_flow_type_version = 1

api_connector_configuration = UserFlowApiConnectorConfiguration()
api_connector_configuration_post_federation_signup = IdentityApiConnector()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}', 
];
apiConnectorConfigurationPostFederationSignup.additionaldata(additionalData)



apiConnectorConfiguration.post_federation_signup = apiConnectorConfigurationPostFederationSignup
api_connector_configuration_post_attribute_collection = IdentityApiConnector()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}', 
];
apiConnectorConfigurationPostAttributeCollection.additionaldata(additionalData)



apiConnectorConfiguration.post_attribute_collection = apiConnectorConfigurationPostAttributeCollection

request_body.api_connector_configuration = apiConnectorConfiguration



result = await client.identity.b2xUserFlows.post(request_body = request_body)


```