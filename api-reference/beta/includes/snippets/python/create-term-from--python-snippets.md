---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Term()
labelsLocalizedLabel1 = LocalizedLabel()
labelsLocalizedLabel1.setLanguageTag('en-US')

labelsLocalizedLabel1.setName('Car')

labelsLocalizedLabel1.setIsDefault(true)


labelsArray []= labelsLocalizedLabel1;
request_body.setLabels(labelsArray)




result = await client.termStore.sets_by_id('set-id').children.post(request_body, headers=)


```