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
		request_body.setDateTime('2021-05-21T21:58:41.327Z')

		request_body.setAtApprovedLocation(null)

notes = Notes()
		notes.setContentType('text')

		notes.setContent('update sample notes')


request_body.setNotes($notes)

request_body.setClockInEvent($clockInEvent)

'clockOutEvent' => request_body = ClockOutEvent()
		request_body.setDateTime('2021-05-21T22:01:46.205Z')

		request_body.setAtApprovedLocation(null)

notes = Notes()
		notes.setContentType('text')

		notes.setContent('update sample notes')


request_body.setNotes($notes)

request_body.setClockOutEvent($clockOutEvent)

'breaks' => breaks1 = ()
		breaks1.setBreakId('BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f')

		breaks1.setNotes(null)

breaks1Start = Start()
		breaks1Start.setDateTime('2021-05-21T21:59:59.328Z')

		breaks1Start.setAtApprovedLocation(null)

breaks1StartNotes = Notes()
		breaks1StartNotes.setContentType('text')

		breaks1StartNotes.setContent('update sample notes')


breaks1Start.setNotes($breaks1StartNotes)

breaks1.setStart($breaks1Start)
breaks1End = End()
		breaks1End.setDateTime('2021-05-21T22:01:10.205Z')

		breaks1End.setAtApprovedLocation(null)

breaks1EndNotes = Notes()
		breaks1EndNotes.setContentType('text')

		breaks1EndNotes.setContent('update sample notes')


breaks1End.setNotes($breaks1EndNotes)

breaks1.setEnd($breaks1End)

breaksArray []= breaks1;
request_body.setBreaks(breaksArray)


];
request_body.setAdditionalData(additionalData)




await client.teams._by_id('team-id').schedule.timeCards._by_id('timeCard-id').put(request_body)


```