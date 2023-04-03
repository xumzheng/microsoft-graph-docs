---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GroupSetting();
valuesSettingValue1 = SettingValue();
valuesSettingValue1.setName('AllowToAddGuests');

valuesSettingValue1.setValue('false');


valuesArray []= valuesSettingValue1;
requestBody.setValues(valuesArray);




result = await client.groupSettingsById('groupSetting-id').patch(requestBody);


```