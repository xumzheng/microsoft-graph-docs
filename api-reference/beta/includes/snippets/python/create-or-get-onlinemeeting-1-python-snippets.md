---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateOrGetPostRequestBody()
request_body.startDateTime = DateTime('2020-02-06T01:49:21.3524945+00:00')

request_body.endDateTime = DateTime('2020-02-06T02:19:21.3524945+00:00')

request_body.subject = 'Create a meeting with customId provided'

request_body.externalId = '7eb8263f-d0e0-4149-bb1c-1f0476083c56'

participants = MeetingParticipants()
attendeesMeetingParticipantInfo1 = MeetingParticipantInfo()
attendeesMeetingParticipantInfo1Identity = IdentitySet()
attendeesMeetingParticipantInfo1IdentityUser = Identity()
attendeesMeetingParticipantInfo1IdentityUser.id = '1f35f2e6-9cab-44ad-8d5a-b74c14720000'


attendeesMeetingParticipantInfo1Identity.user = attendeesMeetingParticipantInfo1IdentityUser

attendeesMeetingParticipantInfo1.identity = attendeesMeetingParticipantInfo1Identity
attendeesMeetingParticipantInfo1.Role(OnlineMeetingRole('presenter'))

attendeesMeetingParticipantInfo1.upn = 'test1@contoso.com'


attendeesArray []= attendeesMeetingParticipantInfo1;
participants.attendees(attendeesArray)



request_body.participants = participants


request_configuration = CreateOrGetRequestBuilderPostRequestConfiguration(
)


result = await client.me.onlineMeetings.createOrGet.post(request_body = request_body)


```