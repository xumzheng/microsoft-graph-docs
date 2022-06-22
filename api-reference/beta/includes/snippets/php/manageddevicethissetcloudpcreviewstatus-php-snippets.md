---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReviewStatusRequestBody();



$reviewStatus = new CloudPcReviewStatus();
$requestRequestBody->setReviewStatus($reviewStatus);


$reviewStatus->setInReview(True);
$reviewStatus->setUserAccessLevel(new CloudPcUserAccessLevel('restricted'));
$reviewStatus->setAzureStorageAccountId('/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview');

$result =  $graphClient->deviceManagement()->managedDevicesById('managedDevice-id')->setCloudPcReviewStatus()->post($requestRequestBody);


```