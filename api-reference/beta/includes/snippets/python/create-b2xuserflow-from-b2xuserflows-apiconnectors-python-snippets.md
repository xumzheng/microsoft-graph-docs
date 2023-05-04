---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2x_identity_user_flow()
request_body.id = 'UserFlowWithAPIConnector'

request_body.userflowtype(UserFlowType.SignUpOrSignIn('userflowtype.signuporsignin'))

request_body.UserFlowTypeVersion = 1

api_connector_configuration = User_flow_api_connector_configuration()
api_connector_configurationpost_federation_signup = Identity_api_connector()
additional_data = [
'@odata_id' => '{apiConnectorId}', 
];
api_connector_configurationpost_federation_signup.additional_data(additional_data)



api_connector_configuration.post_federation_signup = api_connector_configurationpost_federation_signup
api_connector_configurationpost_attribute_collection = Identity_api_connector()
additional_data = [
'@odata_id' => '{apiConnectorId}', 
];
api_connector_configurationpost_attribute_collection.additional_data(additional_data)



api_connector_configuration.post_attribute_collection = api_connector_configurationpost_attribute_collection

request_body.api_connector_configuration = api_connector_configuration



result = await client.identity.b2x_user_flows.post(request_body = request_body)


```