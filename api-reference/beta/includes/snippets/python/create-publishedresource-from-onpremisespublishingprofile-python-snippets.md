---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PublishedResource()
request_body.setDisplayName('New provisioning')

request_body.setResourceName('domain1.contoso.com')



result = await client.onPremisesPublishingProfilesby_id('onPremisesPublishingProfile-id')_publishedResources.post(request_body)


```