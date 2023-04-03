---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CloudPcUserSetting();
requestBody.set@odatatype('#microsoft.graph.cloudPcUserSetting');

requestBody.setDisplayName('Example');

requestBody.setSelfServiceEnabled(false);

requestBody.setLocalAdminEnabled(true);

restorePointSetting = CloudPcRestorePointSetting();
restorePointSetting.setFrequencyInHours(16);

restorePointSetting.setUserRestoreEnabled(true);


requestBody.setRestorePointSetting($restorePointSetting);


result = awaitclient.deviceManagement().virtualEndpoint().userSettings().post(requestBody);


```