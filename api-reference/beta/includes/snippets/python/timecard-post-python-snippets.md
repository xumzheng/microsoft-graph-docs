---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TimeCard()
clock_in_event = TimeCardEvent()
clockInEvent.dateTime = DateTime('2019-03-18T00:00:00.000Z')

clockInEvent.at_approved_location = True

clock_in_event_notes = ItemBody()
clockInEventNotes.content = 'Started late due to traffic in CA 237'

clockInEventNotes.ContentType(BodyType('text'))


clockInEvent.notes = clockInEventNotes

request_body.clock_in_event = clockInEvent
notes = ItemBody()
notes.content = '8 To 5 Inventory management'

notes.ContentType(BodyType('text'))


request_body.notes = notes
breaks_time_card_break1 = TimeCardBreak()
breaksTimeCardBreak1.breakId = 'string'

breaks_time_card_break1_notes = ItemBody()
breaksTimeCardBreak1Notes.content = 'Lunch break'

breaksTimeCardBreak1Notes.ContentType(BodyType('text'))


breaksTimeCardBreak1.notes = breaksTimeCardBreak1Notes
breaks_time_card_break1_start = TimeCardEvent()
breaksTimeCardBreak1Start.dateTime = DateTime('2019-03-18T02:00:00.000Z')

breaksTimeCardBreak1Start.at_approved_location = True

breaks_time_card_break1_start_notes = ItemBody()
breaksTimeCardBreak1StartNotes.content = 'Reduced break to make up for lost time'

breaksTimeCardBreak1StartNotes.ContentType(BodyType('text'))


breaksTimeCardBreak1Start.notes = breaksTimeCardBreak1StartNotes

breaksTimeCardBreak1.start = breaksTimeCardBreak1Start

breaksArray []= breaksTimeCardBreak1;
request_body.breaks(breaksArray)


additionalData = [
'onBehalfOfUserId' => 'a3601044-a1b5-438e-b742-f78d01d68a67', 
];
request_body.additionaldata(additionalData)





result = await client.teams_by_id('team-id').schedule.timeCards.post(request_body = request_body)


```