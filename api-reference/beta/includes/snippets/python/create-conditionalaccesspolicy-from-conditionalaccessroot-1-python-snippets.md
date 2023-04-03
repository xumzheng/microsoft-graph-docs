---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConditionalAccessPolicy();
requestBody.setDisplayName('Access to EXO requires MFA');

requestBody.setState(ConditionalAccessPolicyState('enabled'));

conditions = ConditionalAccessConditionSet();
conditions.setClientAppTypes([conditions.setConditionalAccessClientApp(ConditionalAccessClientApp('mobileappsanddesktopclients'));
conditions.setConditionalAccessClientApp(ConditionalAccessClientApp('browser'));
]);

conditionsApplications = ConditionalAccessApplications();
conditionsApplications.setIncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ]);


conditions.setApplications($conditionsApplications);
conditionsUsers = ConditionalAccessUsers();
conditionsUsers.setIncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ]);


conditions.setUsers($conditionsUsers);
conditionsLocations = ConditionalAccessLocations();
conditionsLocations.setIncludeLocations(['All', ]);

conditionsLocations.setExcludeLocations(['AllTrusted', ]);


conditions.setLocations($conditionsLocations);

requestBody.setConditions($conditions);
grantControls = ConditionalAccessGrantControls();
grantControls.setOperator('OR');

grantControls.setBuiltInControls([grantControls.setConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'));
]);


requestBody.setGrantControls($grantControls);


requestResult = graphServiceClient.identity().conditionalAccess().policies().post(requestBody);


```