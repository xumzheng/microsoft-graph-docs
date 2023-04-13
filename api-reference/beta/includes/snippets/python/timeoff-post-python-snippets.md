---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeOff()
request_body.userId = 'c5d0c76b-80c4-481c-be50-923cd8d680a1'

shared_time_off = TimeOffItem()
sharedTimeOff.timeOffReasonId = 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7'

sharedTimeOff.startDateTime = DateTime('2019-03-11T07:00:00Z')

sharedTimeOff.endDateTime = DateTime('2019-03-12T07:00:00Z')

sharedTimeOff.Theme(ScheduleEntityTheme('white'))


request_body.shared_time_off = sharedTimeOff
draft_time_off = TimeOffItem()
draftTimeOff.timeOffReasonId = 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7'

draftTimeOff.startDateTime = DateTime('2019-03-11T07:00:00Z')

draftTimeOff.endDateTime = DateTime('2019-03-12T07:00:00Z')

draftTimeOff.Theme(ScheduleEntityTheme('pink'))


request_body.draft_time_off = draftTimeOff



result = await client.teams_by_id('team-id').schedule.timesOff.post(request_body = request_body)


```