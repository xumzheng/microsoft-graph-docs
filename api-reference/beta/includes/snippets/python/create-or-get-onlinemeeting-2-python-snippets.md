---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CreateOrGetPostRequestBody();
chatInfo = ChatInfo();
chatInfo.setThreadId('19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2');


request_body.setChatInfo($chatInfo);
request_body.setStartDateTime(DateTime('2020-02-06T01:49:21.3524945+00:00'));

request_body.setEndDateTime(DateTime('2020-02-06T02:19:21.3524945+00:00'));

request_body.setExternalId('7eb8263f-d0e0-4149-bb1c-1f0476083c56');

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



request_body.setParticipants($participants);
request_body.setSubject('Create a meeting with customId provided');



result = await client.me().onlineMeetings().createOrGet().post(request_body);


```