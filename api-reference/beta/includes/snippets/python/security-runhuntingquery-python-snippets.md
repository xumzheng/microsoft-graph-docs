---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RunHuntingQueryPostRequestBody()
request_body.setQuery('DeviceProcessEvents | where InitiatingProcessFileName =~ \"powershell.exe\" | project Timestamp, FileName, InitiatingProcessFileName | order by Timestamp desc | limit 2')



result = await client.security.securityrunHuntingQuery.post(request_body)


```