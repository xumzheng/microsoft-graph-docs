---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Custom_task_extension()
request_body.display_name = 'Grant manager access to mailbox and OneDrive'

request_body.description = 'Grant manager access to mailbox and OneDrive'

endpoint_configuration = Custom_extension_endpoint_configuration()
endpoint_configuration.@odata_type = '#microsoft.graph.logicAppTriggerEndpointConfiguration'

additional_data = [
'subscription_id' => 'c500b67c-e9b7-4ad2-a90d-77d41385ae55', 
'resource_group_name' => 'RG-LCM', 
'logic_app_workflow_name' => 'ManagerAccess', 
];
endpoint_configuration.additional_data(additional_data)



request_body.endpoint_configuration = endpoint_configuration
authentication_configuration = Custom_extension_authentication_configuration()
authentication_configuration.@odata_type = '#microsoft.graph.azureAdTokenAuthentication'

additional_data = [
'resource_id' => '542dc01a-0b5d-4edc-b3f9-5cfe6393f557', 
];
authentication_configuration.additional_data(additional_data)



request_body.authentication_configuration = authentication_configuration
client_configuration = Custom_extension_client_configuration()
client_configuration.@odata_type = '#microsoft.graph.customExtensionClientConfiguration'

client_configuration.TimeoutInMilliseconds = 1000

additional_data = [
'maximum_retries' => 1,
];
client_configuration.additional_data(additional_data)



request_body.client_configuration = client_configuration
callback_configuration = Custom_extension_callback_configuration()
callback_configuration.@odata_type = '#microsoft.graph.identityGovernance.customTaskExtensionCallbackConfiguration'

callback_configuration.timeoutduration =  \DateInterval('PT5M')


request_body.callback_configuration = callback_configuration



result = await client.identity_governance.lifecycle_workflows.custom_task_extensions.post(request_body = request_body)


```