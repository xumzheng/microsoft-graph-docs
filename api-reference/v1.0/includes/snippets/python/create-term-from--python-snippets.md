---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Term()
labelsLocalizedLabel1 = LocalizedLabel()
labelsLocalizedLabel1.languageTag = 'en-US'

labelsLocalizedLabel1.name = 'Car'

labelsLocalizedLabel1.isDefault = true


labelsArray []= labelsLocalizedLabel1;
request_body.labels(labelsArray)




request_configuration = ChildrenRequestBuilderPostRequestConfiguration(
)


result = await client.sites_by_id('site-id').termStore.sets_by_id('set-id').children.post(request_body = request_body)


```