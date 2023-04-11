---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PublishedResource()
request_body.displayName = 'New provisioning'

request_body.resourceName = 'domain1.contoso.com'




result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').publishedResources.post(request_body = request_body)


```