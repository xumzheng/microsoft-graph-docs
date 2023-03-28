---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CloudPcExternalPartnerSetting();
$requestBody.set@odatatype('#microsoft.graph.cloudPcExternalPartnerSetting');

$requestBody.setPartnerId('198d7140-80bb-4843-8cc4-811377a49a92');

$requestBody.setEnableConnection(true);



$requestResult = $graphServiceClient.deviceManagement().virtualEndpoint().externalPartnerSettings().post($requestBody);


```