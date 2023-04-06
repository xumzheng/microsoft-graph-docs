---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetSharedUseLicenseUsageReportPostRequestBody()
request_body.setReportName(CloudPcReportName('shareduselicenseusagereport'))

request_body.setFilter('ServicePlanId eq \'2d1d344e-d10c-41bb-953b-b3a47521dca0\' and DateTimeUTC gt datetime\'2022-11-30\'')

request_body.setSelect(['ServicePlanId', 'LicenseCount', 'ClaimedLicenseCount', 'DateTimeUTC', ])

request_body.setSkip(0)

request_body.setTop(100)


request_config = GetSharedUseLicenseUsageReportRequestBuilderPostRequestConfiguration(
request_config = GetSharedUseLicenseUsageReportRequestBuilderPostRequestConfiguration(query_params=)


await client.deviceManagement.virtualEndpoint.reports.getSharedUseLicenseUsageReport.post(request_body, headers=)


```