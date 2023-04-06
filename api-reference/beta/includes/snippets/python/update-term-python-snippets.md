---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Term()
labelsLocalizedLabel1 = LocalizedLabel()
labelsLocalizedLabel1.setName('changedLabel')

labelsLocalizedLabel1.setLanguageTag('en-US')

labelsLocalizedLabel1.setIsDefault(true)


labelsArray []= labelsLocalizedLabel1;
request_body.setLabels(labelsArray)



request_config = TermRequestBuilderPatchRequestConfiguration(
request_config = TermRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.termStore.sets_by_id('set-id').terms_by_id('term-id').patch(request_body, headers=)


```