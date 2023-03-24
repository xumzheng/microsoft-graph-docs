---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new LifecycleManagementSettings();
$requestBody->setWorkflowScheduleIntervalInHours(3);

$additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity', 
'emailSettings' => $requestBody = new EmailSettings();
$		requestBody->setSenderDomain('ContosoIndustries.net');

		$requestBody->setUseCompanyBranding(true);


$requestBody->setEmailSettings($emailSettings);

];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->identityGovernance()->lifecycleWorkflows()->settings()->patch($requestBody);


```