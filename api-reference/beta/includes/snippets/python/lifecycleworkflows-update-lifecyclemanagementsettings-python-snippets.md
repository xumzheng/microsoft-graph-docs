---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LifecycleManagementSettings()
request_body.workflowScheduleIntervalInHours = 3

emailSettings = EmailSettings()
emailSettings.senderDomain = 'ContosoIndustries.net'

emailSettings.useCompanyBranding = true


request_body.emailSettings = emailSettings
additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
];
request_body.additionaldata(additionalData)




request_configuration = SettingsRequestBuilderPatchRequestConfiguration(
)


result = await client.identityGovernance.lifecycleWorkflows.settings.patch(request_body = request_body)


```