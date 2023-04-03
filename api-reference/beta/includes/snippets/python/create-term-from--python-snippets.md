---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Term();
labelsLocalizedLabel1 = LocalizedLabel();
labelsLocalizedLabel1.setLanguageTag('en-US');

labelsLocalizedLabel1.setName('Car');

labelsLocalizedLabel1.setIsDefault(true);


labelsArray []= labelsLocalizedLabel1;
requestBody.setLabels(labelsArray);




result = awaitclient.termStore().setsById('set-id').children().post(requestBody);


```