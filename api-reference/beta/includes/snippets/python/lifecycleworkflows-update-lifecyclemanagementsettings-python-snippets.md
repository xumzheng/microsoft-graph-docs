---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new LifecycleManagementSettings();
$requestBody->setWorkflowScheduleIntervalInHours(3);

$emailSettings = new EmailSettings();
$emailSettings->setSenderDomain('ContosoIndustries.net');

$emailSettings->setUseCompanyBranding(true);


$requestBody->setEmailSettings($emailSettings);
$additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->identityGovernance()->lifecycleWorkflows()->settings()->patch($requestBody);


```