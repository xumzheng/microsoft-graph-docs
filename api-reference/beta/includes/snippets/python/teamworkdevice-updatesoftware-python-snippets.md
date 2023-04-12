---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateSoftwarePostRequestBody()
request_body.SoftwareType(TeamworkSoftwareType('teamsclient'))

request_body.softwareVersion = '1.0.96.22'




await client.teamwork.devices_by_id('teamworkDevice-id').updateSoftware.post(request_body = request_body)


```