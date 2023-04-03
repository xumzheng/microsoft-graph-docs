---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConditionalAccessPolicy();
requestBody.setDisplayName('Require MFA to EXO from non-compliant devices.');

requestBody.setState(ConditionalAccessPolicyState('enabled'));

conditions = ConditionalAccessConditionSet();
conditionsApplications = ConditionalAccessApplications();
conditionsApplications.setIncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ]);


conditions.setApplications($conditionsApplications);
conditionsUsers = ConditionalAccessUsers();
conditionsUsers.setIncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ]);


conditions.setUsers($conditionsUsers);

requestBody.setConditions($conditions);
grantControls = ConditionalAccessGrantControls();
grantControls.setOperator('OR');

grantControls.setBuiltInControls([grantControls.setConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'));
]);


requestBody.setGrantControls($grantControls);


result = await client.identity().conditionalAccess().policies().post(requestBody);


```