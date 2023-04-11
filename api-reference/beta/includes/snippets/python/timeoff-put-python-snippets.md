---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimesOff()
additionalData = [
'userId' => 'c5d0c76b-80c4-481c-be50-923cd8d680a1', 
'sharedTimeOff' => request_body = SharedTimeOff()
		request_body.timeOffReasonId = 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7'

		request_body.startDateTime = '2019-03-11T07:00:00Z'

		request_body.endDateTime = '2019-03-12T07:00:00Z'

		request_body.theme = 'white'


request_body.sharedTimeOff = sharedTimeOff

'draftTimeOff' => request_body = DraftTimeOff()
		request_body.timeOffReasonId = 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7'

		request_body.startDateTime = '2019-03-11T07:00:00Z'

		request_body.endDateTime = '2019-03-12T07:00:00Z'

		request_body.theme = 'pink'


request_body.draftTimeOff = draftTimeOff

];
request_body.additionaldata(additionalData)




request_configuration = TimeOffRequestBuilderPutRequestConfiguration(
headers = {
					'Prefer' : "return=representation",
}

)


await client.teams_by_id('team-id').schedule.timesOff_by_id('timeOff-id').put(request_body = request_body, request_configuration = request_configuration)


```