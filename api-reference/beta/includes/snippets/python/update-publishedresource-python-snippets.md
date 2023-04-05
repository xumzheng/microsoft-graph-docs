---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PublishedResource()
request_body.setDisplayName('Demo provisioning (updated)')



result = await client.onPremisesPublishingProfiles._by_id('onPremisesPublishingProfile-id').publishedResources._by_id('publishedResource-id').patch(request_body)


```