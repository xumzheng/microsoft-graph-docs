---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConditionalAccessPolicy();
requestBody.setDisplayName('Block access to EXO non-trusted regions.');

requestBody.setState(ConditionalAccessPolicyState('enabled'));

conditions = ConditionalAccessConditionSet();
conditions.setClientAppTypes([conditions.setConditionalAccessClientApp(ConditionalAccessClientApp('all'));
]);

conditionsApplications = ConditionalAccessApplications();
conditionsApplications.setIncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ]);


conditions.setApplications($conditionsApplications);
conditionsUsers = ConditionalAccessUsers();
conditionsUsers.setIncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ]);


conditions.setUsers($conditionsUsers);
conditionsLocations = ConditionalAccessLocations();
conditionsLocations.setIncludeLocations(['198ad66e-87b3-4157-85a3-8a7b51794ee9', ]);


conditions.setLocations($conditionsLocations);

requestBody.setConditions($conditions);
grantControls = ConditionalAccessGrantControls();
grantControls.setOperator('OR');

grantControls.setBuiltInControls([grantControls.setConditionalAccessGrantControl(ConditionalAccessGrantControl('block'));
]);


requestBody.setGrantControls($grantControls);


result = awaitclient.identity().conditionalAccess().policies().post(requestBody);


```