---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OnlineMeeting();
$requestBody.setStartDateTime(new DateTime('2019-07-12T14:30:34.2444915-07:00'));

$requestBody.setEndDateTime(new DateTime('2019-07-12T15:00:34.2464912-07:00'));

$requestBody.setSubject('User meeting');

$joinMeetingIdSettings = new JoinMeetingIdSettings();
$joinMeetingIdSettings.setIsPasscodeRequired(true);


$requestBody.setJoinMeetingIdSettings($joinMeetingIdSettings);


$requestResult = $graphServiceClient.me().onlineMeetings().post($requestBody);


```