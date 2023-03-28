---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConditionalAccessPolicy();
$requestBody->setDisplayName('Policy for risky sign-in');

$requestBody->setState(new ConditionalAccessPolicyState('enabled'));

$conditions = new ConditionalAccessConditionSet();
$conditions->setSignInRiskLevels([$conditions->setRiskLevel(new RiskLevel('high'));
$conditions->setRiskLevel(new RiskLevel('medium'));
]);

$conditionsApplications = new ConditionalAccessApplications();
$conditionsApplications->setIncludeApplications(['All', ]);


$conditions->setApplications($conditionsApplications);
$conditionsUsers = new ConditionalAccessUsers();
$conditionsUsers->setIncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ]);


$conditions->setUsers($conditionsUsers);

$requestBody->setConditions($conditions);
$grantControls = new ConditionalAccessGrantControls();
$grantControls->setOperator('OR');

$grantControls->setBuiltInControls([$grantControls->setConditionalAccessGrantControl(new ConditionalAccessGrantControl('mfa'));
]);


$requestBody->setGrantControls($grantControls);


$requestResult = $graphServiceClient->identity()->conditionalAccess()->policies()->post($requestBody);


```