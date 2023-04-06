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
		request_body.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7')

		request_body.setStartDateTime('2019-03-11T07:00:00Z')

		request_body.setEndDateTime('2019-03-12T07:00:00Z')

		request_body.setTheme('white')


request_body.setSharedTimeOff($sharedTimeOff)

'draftTimeOff' => request_body = DraftTimeOff()
		request_body.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7')

		request_body.setStartDateTime('2019-03-11T07:00:00Z')

		request_body.setEndDateTime('2019-03-12T07:00:00Z')

		request_body.setTheme('pink')


request_body.setDraftTimeOff($draftTimeOff)

];
request_body.setAdditionalData(additionalData)



request_config = TimeOffRequestBuilderPutRequestConfiguration(
request_config = TimeOffRequestBuilderPutRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


await client.teams_by_id('team-id').schedule.timesOff_by_id('timeOff-id').put(request_body, request_config, headers=request_config)


```