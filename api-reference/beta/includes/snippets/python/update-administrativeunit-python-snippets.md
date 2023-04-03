---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AdministrativeUnit();
additionalData = [
'membershipType' => 'Dynamic', 
'membershipRule' => '(user.country -eq \"United States\")', 
'membershipRuleProcessingState' => 'On', 
];
requestBody.setAdditionalData(additionalData);




result = await client.administrativeUnitsById('administrativeUnit-id').patch(requestBody);


```