---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GroupSetting()
valuesSettingValue1 = SettingValue()
valuesSettingValue1.setName('AllowToAddGuests')

valuesSettingValue1.setValue('false')


valuesArray []= valuesSettingValue1;
request_body.setValues(valuesArray)



request_config = GroupSettingRequestBuilderPatchRequestConfiguration(
request_config = GroupSettingRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.groupSettings_by_id('groupSetting-id').patch(request_body, headers=)


```