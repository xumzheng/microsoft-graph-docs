---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PublishedResource();
requestBody.setDisplayName('Demo provisioning (updated)');



result = awaitclient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').publishedResourcesById('publishedResource-id').patch(requestBody);


```