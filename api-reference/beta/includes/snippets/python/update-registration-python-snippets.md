---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MeetingRegistration()
request_body.subject = 'Microsoft Ignite: Day 1'

request_body.startDateTime = DateTime('2021-11-02T08:00:00-08:00')

request_body.endDateTime = DateTime('2021-11-02T15:45:00-08:00')

speakers_meeting_speaker1 = MeetingSpeaker()
speakersMeetingSpeaker1.displayName = 'Henry Ross'

speakersMeetingSpeaker1.bio = 'Chairman and Chief Executive Officer'


speakersArray []= speakersMeetingSpeaker1;
speakers_meeting_speaker2 = MeetingSpeaker()
speakersMeetingSpeaker2.displayName = 'Fred Ryan'

speakersMeetingSpeaker2.bio = 'CVP'


speakersArray []= speakersMeetingSpeaker2;
request_body.speakers(speakersArray)





result = await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.patch(request_body = request_body)


```