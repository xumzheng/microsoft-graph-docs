---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SetCloudPcReviewStatusPostRequestBody()
reviewStatus = CloudPcReviewStatus()
reviewStatus.inReview = true

reviewStatus.UserAccessLevel(CloudPcUserAccessLevel('restricted'))

reviewStatus.azureStorageAccountId = '/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview'


request_body.reviewStatus = reviewStatus


request_configuration = SetCloudPcReviewStatusRequestBuilderPostRequestConfiguration(
)


await client.deviceManagement.managedDevices_by_id('managedDevice-id').setCloudPcReviewStatus.post(request_body = request_body)


```