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
request_body.setAdditionalData(additionalData)



request_config = TimeOffReasonRequestBuilderPutRequestConfiguration()

headers = [
	'Prefer' => 'return=representation',
]

request_config.headers = headers


await client.teams._by_id('team-id').schedule.timeOffReasons._by_id('timeOffReason-id').put(request_body, request_config)


```