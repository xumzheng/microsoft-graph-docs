---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AdministrativeUnit();
additionalData = [
'membershipType' => 'Dynamic', 
'membershipRule' => '(user.country -eq \"United States\")', 
'membershipRuleProcessingState' => 'On', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.administrativeUnitsById('administrativeUnit-id').patch(requestBody);


```