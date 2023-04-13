---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Term()
labels_localized_label1 = LocalizedLabel()
labelsLocalizedLabel1.name = 'changedLabel'

labelsLocalizedLabel1.languageTag = 'en-US'

labelsLocalizedLabel1.is_default = True


labelsArray []= labelsLocalizedLabel1;
request_body.labels(labelsArray)





result = await client.termStore.sets_by_id('set-id').terms_by_id('term-id').patch(request_body = request_body)


```