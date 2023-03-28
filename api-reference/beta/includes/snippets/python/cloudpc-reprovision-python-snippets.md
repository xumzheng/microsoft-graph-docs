---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReprovisionPostRequestBody();
$requestBody->setUserAccountType(new CloudPcUserAccountType('administrator'));

$requestBody->setOsVersion(new CloudPcOperatingSystem('windows10'));



$graphServiceClient->deviceManagement()->virtualEndpoint()->cloudPCsById('cloudPC-id')->reprovision()->post($requestBody);


```