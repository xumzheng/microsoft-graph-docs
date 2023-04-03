---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OnlineMeeting();
requestBody.setStartDateTime(DateTime('2019-07-12T14:30:34.2444915-07:00'));

requestBody.setEndDateTime(DateTime('2019-07-12T15:00:34.2464912-07:00'));

requestBody.setSubject('User meeting');

joinMeetingIdSettings = JoinMeetingIdSettings();
joinMeetingIdSettings.setIsPasscodeRequired(true);


requestBody.setJoinMeetingIdSettings($joinMeetingIdSettings);


result = awaitclient.me().onlineMeetings().post(requestBody);


```