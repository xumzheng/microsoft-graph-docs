---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeOffReason()
additionalData = [
'displayName' => 'Vacation', 
'iconType' => 'plane', 
'isActive' => true,
];
request_body.additionaldata(additionalData)




request_configuration = TimeOffReasonRequestBuilderPutRequestConfiguration(
headers = {
					'Prefer' : "return=representation",
}

)


await client.teams_by_id('team-id').schedule.timeOffReasons_by_id('timeOffReason-id').put(request_body = request_body, request_configuration = request_configuration)


```