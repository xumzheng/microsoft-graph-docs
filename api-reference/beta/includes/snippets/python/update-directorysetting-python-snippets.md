---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DirectorySetting();
valuesSettingValue1 = SettingValue();
valuesSettingValue1.setName('CustomBlockedWordsList');

valuesSettingValue1.setValue('Contoso');


valuesArray []= valuesSettingValue1;
requestBody.setValues(valuesArray);




result = await client.settingsById('directorySetting-id').patch(requestBody);


```