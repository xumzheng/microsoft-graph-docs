---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Lifecycle_management_settings()
request_body.WorkflowScheduleIntervalInHours = 3

email_settings = Email_settings()
email_settings.sender_domain = 'ContosoIndustries.net'

email_settings.use_company_branding = True


request_body.email_settings = email_settings
additional_data = [
'@odata_context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
];
request_body.additional_data(additional_data)





result = await client.identity_governance.lifecycle_workflows.settings.patch(request_body = request_body)


```