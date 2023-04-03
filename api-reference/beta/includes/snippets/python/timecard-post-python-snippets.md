---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = TimeCard();
clockInEvent = TimeCardEvent();
clockInEvent.setDateTime(DateTime('2019-03-18T00:00:00.000Z'));

clockInEvent.setAtApprovedLocation(true);

clockInEventNotes = ItemBody();
clockInEventNotes.setContent('Started late due to traffic in CA 237');

clockInEventNotes.setContentType(BodyType('text'));


clockInEvent.setNotes($clockInEventNotes);

requestBody.setClockInEvent($clockInEvent);
notes = ItemBody();
notes.setContent('8 To 5 Inventory management');

notes.setContentType(BodyType('text'));


requestBody.setNotes($notes);
breaksTimeCardBreak1 = TimeCardBreak();
breaksTimeCardBreak1.setBreakId('string');

breaksTimeCardBreak1Notes = ItemBody();
breaksTimeCardBreak1Notes.setContent('Lunch break');

breaksTimeCardBreak1Notes.setContentType(BodyType('text'));


breaksTimeCardBreak1.setNotes($breaksTimeCardBreak1Notes);
breaksTimeCardBreak1Start = TimeCardEvent();
breaksTimeCardBreak1Start.setDateTime(DateTime('2019-03-18T02:00:00.000Z'));

breaksTimeCardBreak1Start.setAtApprovedLocation(true);

breaksTimeCardBreak1StartNotes = ItemBody();
breaksTimeCardBreak1StartNotes.setContent('Reduced break to make up for lost time');

breaksTimeCardBreak1StartNotes.setContentType(BodyType('text'));


breaksTimeCardBreak1Start.setNotes($breaksTimeCardBreak1StartNotes);

breaksTimeCardBreak1.setStart($breaksTimeCardBreak1Start);

breaksArray []= breaksTimeCardBreak1;
requestBody.setBreaks(breaksArray);


additionalData = [
'onBehalfOfUserId' => 'a3601044-a1b5-438e-b742-f78d01d68a67', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.teamsById('team-id').schedule().timeCards().post(requestBody);


```