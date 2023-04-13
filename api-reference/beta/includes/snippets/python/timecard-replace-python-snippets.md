---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeCard()
additionalData = [
'userId' => '70e47528-2fae-42b5-9d8e-ee73ccd90603', 
'state' => 'clockedOut', 
'confirmedBy' => 'None', 
'notes' => 		null,
'clockInEvent' => request_body = ClockInEvent()
		request_body.dateTime = '2021-05-21T21:58:41.327Z'

		request_body.atApprovedLocation=null

notes = Notes()
		notes.contentType = 'text'

		notes.content = 'update sample notes'


request_body.notes = notes

request_body.clock_in_event = clockInEvent

'clockOutEvent' => request_body = ClockOutEvent()
		request_body.dateTime = '2021-05-21T22:01:46.205Z'

		request_body.atApprovedLocation=null

notes = Notes()
		notes.contentType = 'text'

		notes.content = 'update sample notes'


request_body.notes = notes

request_body.clock_out_event = clockOutEvent

'breaks' => breaks1 = ()
		breaks1.breakId = 'BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f'

		breaks1.notes=null

breaks1_start = Start()
		breaks1Start.dateTime = '2021-05-21T21:59:59.328Z'

		breaks1Start.atApprovedLocation=null

breaks1_start_notes = Notes()
		breaks1StartNotes.contentType = 'text'

		breaks1StartNotes.content = 'update sample notes'


breaks1Start.notes = breaks1StartNotes

breaks1.start = breaks1Start
breaks1_end = End()
		breaks1End.dateTime = '2021-05-21T22:01:10.205Z'

		breaks1End.atApprovedLocation=null

breaks1_end_notes = Notes()
		breaks1EndNotes.contentType = 'text'

		breaks1EndNotes.content = 'update sample notes'


breaks1End.notes = breaks1EndNotes

breaks1.end = breaks1End

breaksArray []= breaks1;
request_body.breaks(breaksArray)


];
request_body.additionaldata(additionalData)





await client.teams_by_id('team-id').schedule.timeCards_by_id('timeCard-id').put(request_body = request_body)


```