---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ActivityBasedTimeoutPolicy();
requestBody.setDefinition(['definition-value', ]);

requestBody.setDisplayName('displayName-value');

requestBody.setIsOrganizationDefault(true);



result = await client.policies().activityBasedTimeoutPoliciesById('activityBasedTimeoutPolicy-id').patch(requestBody);


```