---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PublishedResource();
requestBody.setDisplayName('Demo provisioning (updated)');



requestResult = graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').publishedResourcesById('publishedResource-id').patch(requestBody);


```