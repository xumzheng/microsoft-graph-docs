---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnlineMeeting()
request_body.setStartDateTime(DateTime('2019-07-12T14:30:34.2444915-07:00'))

request_body.setEndDateTime(DateTime('2019-07-12T15:00:34.2464912-07:00'))

request_body.setSubject('User meeting in Microsoft Teams channel.')

joinMeetingIdSettings = JoinMeetingIdSettings()
joinMeetingIdSettings.setIsPasscodeRequired(false)


request_body.setJoinMeetingIdSettings($joinMeetingIdSettings)

request_config = OnlineMeetingsRequestBuilderPostRequestConfiguration(
request_config = OnlineMeetingsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.onlineMeetings.post(request_body, headers=)


```