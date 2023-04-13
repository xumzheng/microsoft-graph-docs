---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
request_body.displayName = 'Seattle District Technical Schools'

request_body.description = 'Seattle district technical schools administration'

additionalData = [
'membershipType' => 'Dynamic', 
'membershipRule' => '(user.country -eq \"United States\")', 
'membershipRuleProcessingState' => 'On', 
];
request_body.additionaldata(additionalData)





result = await client.administrativeUnits.post(request_body = request_body)


```