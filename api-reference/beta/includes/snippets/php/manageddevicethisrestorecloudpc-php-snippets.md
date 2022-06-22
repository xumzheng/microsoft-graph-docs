---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcSnapshotIdRequestBody();


$requestRequestBody->setCloudPcSnapshotId('A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8');
$result =  $graphClient->deviceManagement()->managedDevicesById('managedDevice-id')->restoreCloudPc()->post($requestRequestBody);


```