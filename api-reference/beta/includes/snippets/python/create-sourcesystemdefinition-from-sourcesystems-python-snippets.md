---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Source_system_definition()
request_body.display_name = 'Rostering source'

user_matching_settings_user_matching_setting1 = User_matching_setting()
user_matching_settings_user_matching_setting1match_target = User_match_target_reference_value()
user_matching_settings_user_matching_setting1match_target.code = 'userPrincipalName'


user_matching_settings_user_matching_setting1.match_target = user_matching_settings_user_matching_setting1match_target
user_matching_settings_user_matching_setting1.PriorityOrder = 0

user_matching_settings_user_matching_setting1source_identifier = Identifier_type_reference_value()
user_matching_settings_user_matching_setting1source_identifier.code = 'username'


user_matching_settings_user_matching_setting1.source_identifier = user_matching_settings_user_matching_setting1source_identifier
additional_data = [
'role_group@odata_bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups/staff', 
];
user_matching_settings_user_matching_setting1.additional_data(additional_data)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting1;
user_matching_settings_user_matching_setting2 = User_matching_setting()
user_matching_settings_user_matching_setting2match_target = User_match_target_reference_value()
user_matching_settings_user_matching_setting2match_target.code = 'userPrincipalName'


user_matching_settings_user_matching_setting2.match_target = user_matching_settings_user_matching_setting2match_target
user_matching_settings_user_matching_setting2.PriorityOrder = 1

user_matching_settings_user_matching_setting2source_identifier = Identifier_type_reference_value()
user_matching_settings_user_matching_setting2source_identifier.code = 'username'


user_matching_settings_user_matching_setting2.source_identifier = user_matching_settings_user_matching_setting2source_identifier
additional_data = [
'role_group@odata_bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups(\'students\')', 
];
user_matching_settings_user_matching_setting2.additional_data(additional_data)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting2;
request_body.usermatchingsettings(userMatchingSettingsArray)





result = await client.external.industry_data.source_systems.post(request_body = request_body)


```