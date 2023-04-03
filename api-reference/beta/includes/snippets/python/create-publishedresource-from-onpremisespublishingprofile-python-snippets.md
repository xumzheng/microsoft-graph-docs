---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PublishedResource();
requestBody.setDisplayName('New provisioning');

requestBody.setResourceName('domain1.contoso.com');



result = awaitclient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').publishedResources().post(requestBody);


```