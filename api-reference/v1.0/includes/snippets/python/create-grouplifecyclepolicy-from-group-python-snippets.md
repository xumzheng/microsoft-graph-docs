---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GroupLifecyclePolicy();
$requestBody.setGroupLifetimeInDays(100);

$requestBody.setManagedGroupTypes('Selected');

$requestBody.setAlternateNotificationEmails('admin@contoso.com');



$requestResult = $graphServiceClient.groupLifecyclePolicies().post($requestBody);


```