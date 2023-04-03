---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConditionalAccessPolicy();
requestBody.setDisplayName('Policy for risky sign-in');

requestBody.setState(ConditionalAccessPolicyState('enabled'));

conditions = ConditionalAccessConditionSet();
conditions.setSignInRiskLevels([conditions.setRiskLevel(RiskLevel('high'));
conditions.setRiskLevel(RiskLevel('medium'));
]);

conditionsApplications = ConditionalAccessApplications();
conditionsApplications.setIncludeApplications(['All', ]);


conditions.setApplications($conditionsApplications);
conditionsUsers = ConditionalAccessUsers();
conditionsUsers.setIncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ]);


conditions.setUsers($conditionsUsers);

requestBody.setConditions($conditions);
grantControls = ConditionalAccessGrantControls();
grantControls.setOperator('OR');

grantControls.setBuiltInControls([grantControls.setConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'));
]);


requestBody.setGrantControls($grantControls);


result = await client.identity().conditionalAccess().policies().post(requestBody);


```