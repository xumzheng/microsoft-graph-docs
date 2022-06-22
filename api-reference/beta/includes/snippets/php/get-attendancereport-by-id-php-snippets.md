---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MeetingAttendanceReportRequestBuilderGetRequestConfiguration();

$queryParameters = new MeetingAttendanceReportRequestBuilderGetQueryParameters();
$queryParameters->expand = 'attendanceRecords';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->attendanceReportsById('meetingAttendanceReport-id')->get($requestConfiguration);


```