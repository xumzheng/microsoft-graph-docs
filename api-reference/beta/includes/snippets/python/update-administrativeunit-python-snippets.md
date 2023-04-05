---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
additionalData = [
'membershipType' => 'Dynamic', 
'membershipRule' => '(user.country -eq \"United States\")', 
'membershipRuleProcessingState' => 'On', 
];
request_body.setAdditionalData(additionalData)




result = await client.administrativeUnitsById('administrativeUnit-id').patch(request_body)


```