---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeOff()
request_body.setUserId('c5d0c76b-80c4-481c-be50-923cd8d680a1')

sharedTimeOff = TimeOffItem()
sharedTimeOff.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7')

sharedTimeOff.setStartDateTime(DateTime('2019-03-11T07:00:00Z'))

sharedTimeOff.setEndDateTime(DateTime('2019-03-12T07:00:00Z'))

sharedTimeOff.setTheme(ScheduleEntityTheme('white'))


request_body.setSharedTimeOff($sharedTimeOff)
draftTimeOff = TimeOffItem()
draftTimeOff.setTimeOffReasonId('TOR_891045ca-b5d2-406b-aa06-a3c8921245d7')

draftTimeOff.setStartDateTime(DateTime('2019-03-11T07:00:00Z'))

draftTimeOff.setEndDateTime(DateTime('2019-03-12T07:00:00Z'))

draftTimeOff.setTheme(ScheduleEntityTheme('pink'))


request_body.setDraftTimeOff($draftTimeOff)


result = await client.teams_by_id('team-id').schedule.timesOff.post(request_body, headers=)


```