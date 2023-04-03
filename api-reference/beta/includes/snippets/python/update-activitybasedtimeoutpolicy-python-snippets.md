---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ActivityBasedTimeoutPolicy();
requestBody.setDefinition(['definition-value', ]);

requestBody.setDisplayName('displayName-value');

requestBody.setIsOrganizationDefault(true);



requestResult = graphServiceClient.policies().activityBasedTimeoutPoliciesById('activityBasedTimeoutPolicy-id').patch(requestBody);


```