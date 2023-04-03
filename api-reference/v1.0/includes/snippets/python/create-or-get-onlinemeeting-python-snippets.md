---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CreateOrGetPostRequestBody();
requestBody.setStartDateTime(DateTime('2020-02-06T01:49:21.3524945+00:00'));

requestBody.setEndDateTime(DateTime('2020-02-06T02:19:21.3524945+00:00'));

requestBody.setSubject('Create a meeting with customId provided');

requestBody.setExternalId('7eb8263f-d0e0-4149-bb1c-1f0476083c56');

participants = MeetingParticipants();
attendeesMeetingParticipantInfo1 = MeetingParticipantInfo();
attendeesMeetingParticipantInfo1Identity = IdentitySet();
attendeesMeetingParticipantInfo1IdentityUser = Identity();
attendeesMeetingParticipantInfo1IdentityUser.setId('1f35f2e6-9cab-44ad-8d5a-b74c14720000');


attendeesMeetingParticipantInfo1Identity.setUser($attendeesMeetingParticipantInfo1IdentityUser);

attendeesMeetingParticipantInfo1.setIdentity($attendeesMeetingParticipantInfo1Identity);
attendeesMeetingParticipantInfo1.setUpn('test1@contoso.com');


attendeesArray []= attendeesMeetingParticipantInfo1;
participants.setAttendees(attendeesArray);



requestBody.setParticipants($participants);


result = await client.me().onlineMeetings().createOrGet().post(requestBody);


```