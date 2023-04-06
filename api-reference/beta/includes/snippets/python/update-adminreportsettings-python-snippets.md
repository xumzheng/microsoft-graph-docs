---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdminReportSettings()
request_body.setDisplayConcealedNames(true)


request_config = ReportSettingsRequestBuilderPatchRequestConfiguration(
request_config = ReportSettingsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.admin.reportSettings.patch(request_body, headers=)


```