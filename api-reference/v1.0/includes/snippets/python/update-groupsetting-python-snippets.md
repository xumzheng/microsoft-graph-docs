---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GroupSetting()
valuesSettingValue1 = SettingValue()
valuesSettingValue1.name = 'AllowToAddGuests'

valuesSettingValue1.value = 'true'


valuesArray []= valuesSettingValue1;
request_body.values(valuesArray)




request_configuration = GroupSettingRequestBuilderPatchRequestConfiguration(
)


result = await client.groups_by_id('group-id').settings_by_id('groupSetting-id').patch(request_body = request_body)


```