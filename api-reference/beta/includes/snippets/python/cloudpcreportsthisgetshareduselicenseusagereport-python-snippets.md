---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetSharedUseLicenseUsageReportPostRequestBody()
request_body.ReportName(CloudPcReportName('shareduselicenseusagereport'))

request_body.filter = 'ServicePlanId eq \'2d1d344e-d10c-41bb-953b-b3a47521dca0\' and DateTimeUTC gt datetime\'2022-11-30\''

request_body.Select(['ServicePlanId', 'LicenseCount', 'ClaimedLicenseCount', 'DateTimeUTC', ])

request_body.skip = 0

request_body.top = 100



request_configuration = GetSharedUseLicenseUsageReportRequestBuilderPostRequestConfiguration(
)


await client.deviceManagement.virtualEndpoint.reports.getSharedUseLicenseUsageReport.post(request_body = request_body)


```