---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SetCloudPcReviewStatusPostRequestBody();
reviewStatus = CloudPcReviewStatus();
reviewStatus.setInReview(true);

reviewStatus.setUserAccessLevel(CloudPcUserAccessLevel('restricted'));

reviewStatus.setAzureStorageAccountId('/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview');


requestBody.setReviewStatus($reviewStatus);


graphServiceClient.deviceManagement().managedDevicesById('managedDevice-id').setCloudPcReviewStatus().post(requestBody);


```