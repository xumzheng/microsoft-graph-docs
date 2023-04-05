---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = MeetingAttendanceReportRequestBuilderGetRequestConfiguration()

query_params = MeetingAttendanceReportRequestBuilderGetQueryParameters()
query_params.expand = ["attendanceRecords"]

request_config.queryParameters = query_params


result = await client.me.onlineMeetings._by_id('onlineMeeting-id').attendanceReports._by_id('meetingAttendanceReport-id').get(request_config)


```