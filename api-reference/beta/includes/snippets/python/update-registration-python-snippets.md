---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MeetingRegistration();
requestBody.setSubject('Microsoft Ignite: Day 1');

requestBody.setStartDateTime(DateTime('2021-11-02T08:00:00-08:00'));

requestBody.setEndDateTime(DateTime('2021-11-02T15:45:00-08:00'));

speakersMeetingSpeaker1 = MeetingSpeaker();
speakersMeetingSpeaker1.setDisplayName('Henry Ross');

speakersMeetingSpeaker1.setBio('Chairman and Chief Executive Officer');


speakersArray []= speakersMeetingSpeaker1;
speakersMeetingSpeaker2 = MeetingSpeaker();
speakersMeetingSpeaker2.setDisplayName('Fred Ryan');

speakersMeetingSpeaker2.setBio('CVP');


speakersArray []= speakersMeetingSpeaker2;
requestBody.setSpeakers(speakersArray);




result = await client.me().onlineMeetingsById('onlineMeeting-id').registration().patch(requestBody);


```