---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = MeetingAttendanceReportRequestBuilderGetRequestConfiguration(
request_configuration = MeetingAttendanceReportRequestBuilderGetRequestConfiguration(query_params=query_params = MeetingAttendanceReportRequestBuilderGetQueryParameters()
query_params['expand'] = ["attendanceRecords"]

)
query_params = MeetingAttendanceReportRequestBuilderGetQueryParameters()
query_params['expand'] = ["attendanceRecords"]

)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').attendanceReports_by_id('meetingAttendanceReport-id').get(request_configuration)


```