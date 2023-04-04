---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = LifecycleManagementSettings();
request_body.setWorkflowScheduleIntervalInHours(3);

emailSettings = EmailSettings();
emailSettings.setSenderDomain('ContosoIndustries.net');

emailSettings.setUseCompanyBranding(true);


request_body.setEmailSettings($emailSettings);
additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
];
request_body.setAdditionalData(additionalData);




result = await client.identityGovernance.lifecycleWorkflows.settings.patch(request_body);


```