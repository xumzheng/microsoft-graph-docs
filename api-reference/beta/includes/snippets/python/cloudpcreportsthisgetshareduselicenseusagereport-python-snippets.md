---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetSharedUseLicenseUsageReportPostRequestBody();
requestBody.setReportName(CloudPcReportName('shareduselicenseusagereport'));

requestBody.setFilter('ServicePlanId eq \'2d1d344e-d10c-41bb-953b-b3a47521dca0\' and DateTimeUTC gt datetime\'2022-11-30\'');

requestBody.setSelect(['ServicePlanId', 'LicenseCount', 'ClaimedLicenseCount', 'DateTimeUTC', ]);

requestBody.setSkip(0);

requestBody.setTop(100);



await client.deviceManagement().virtualEndpoint().reports().getSharedUseLicenseUsageReport().post(requestBody);


```