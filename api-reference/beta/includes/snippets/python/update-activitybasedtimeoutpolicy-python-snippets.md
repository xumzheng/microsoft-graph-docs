---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ActivityBasedTimeoutPolicy();
$requestBody.setDefinition(['definition-value', ]);

$requestBody.setDisplayName('displayName-value');

$requestBody.setIsOrganizationDefault(true);



$requestResult = $graphServiceClient.policies().activityBasedTimeoutPoliciesById('activityBasedTimeoutPolicy-id').patch($requestBody);


```