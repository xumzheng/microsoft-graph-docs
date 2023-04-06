---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MeetingAttendanceReportRequestBuilderGetRequestConfiguration(
request_config = MeetingAttendanceReportRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["attendanceRecords"]
)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').attendanceReports_by_id('meetingAttendanceReport-id').get(request_config, headers=request_config)


```