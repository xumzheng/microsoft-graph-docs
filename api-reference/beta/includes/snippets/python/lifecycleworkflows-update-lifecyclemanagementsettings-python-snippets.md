---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LifecycleManagementSettings()
request_body.workflow_schedule_interval_in_hours = 3

email_settings = EmailSettings()
emailSettings.senderDomain = 'ContosoIndustries.net'

emailSettings.use_company_branding = True


request_body.email_settings = emailSettings
additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.lifecycleWorkflows.settings.patch(request_body = request_body)


```