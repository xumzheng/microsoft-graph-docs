---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = MeetingAttendanceReportRequestBuilder.MeetingAttendanceReportRequestBuilderGetQueryParameters(
		expand = ["attendanceRecords"],
)

request_configuration = MeetingAttendanceReportRequestBuilder.MeetingAttendanceReportRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').attendanceReports_by_id('meetingAttendanceReport-id').get(request_configuration = request_configuration)


```