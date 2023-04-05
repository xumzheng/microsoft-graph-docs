---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetCloudPcReviewStatusPostRequestBody()
reviewStatus = CloudPcReviewStatus()
reviewStatus.setInReview(true)

reviewStatus.setUserAccessLevel(CloudPcUserAccessLevel('restricted'))

reviewStatus.setAzureStorageAccountId('/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview')


request_body.setReviewStatus($reviewStatus)


await client.deviceManagement.managedDevices._by_id('managedDevice-id').setCloudPcReviewStatus.post(request_body)


```