---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = GroupSetting();
valuesSettingValue1 = SettingValue();
valuesSettingValue1.setName('AllowToAddGuests');

valuesSettingValue1.setValue('true');


valuesArray []= valuesSettingValue1;
requestBody.setValues(valuesArray);




requestResult = graphServiceClient.groupsById('group-id').settingsById('groupSetting-id').patch(requestBody);


```