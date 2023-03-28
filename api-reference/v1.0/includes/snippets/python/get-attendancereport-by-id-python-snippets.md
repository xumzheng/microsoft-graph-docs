---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new MeetingAttendanceReportRequestBuilderGetRequestConfiguration();

$queryParameters = new MeetingAttendanceReportRequestBuilderGetQueryParameters();
$queryParameters.expand = ["attendanceRecords"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').attendanceReportsById('meetingAttendanceReport-id').get($requestConfiguration);


```