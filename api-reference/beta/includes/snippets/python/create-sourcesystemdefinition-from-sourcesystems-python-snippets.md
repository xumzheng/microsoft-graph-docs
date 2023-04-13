---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceSystemDefinition()
request_body.displayName = 'Rostering source'

user_matching_settings_user_matching_setting1 = UserMatchingSetting()
user_matching_settings_user_matching_setting1_match_target = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting1MatchTarget.code = 'userPrincipalName'


userMatchingSettingsUserMatchingSetting1.match_target = userMatchingSettingsUserMatchingSetting1MatchTarget
userMatchingSettingsUserMatchingSetting1.priority_order = 0

user_matching_settings_user_matching_setting1_source_identifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting1SourceIdentifier.code = 'username'


userMatchingSettingsUserMatchingSetting1.source_identifier = userMatchingSettingsUserMatchingSetting1SourceIdentifier
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups/staff', 
];
userMatchingSettingsUserMatchingSetting1.additionaldata(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting1;
user_matching_settings_user_matching_setting2 = UserMatchingSetting()
user_matching_settings_user_matching_setting2_match_target = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting2MatchTarget.code = 'userPrincipalName'


userMatchingSettingsUserMatchingSetting2.match_target = userMatchingSettingsUserMatchingSetting2MatchTarget
userMatchingSettingsUserMatchingSetting2.priority_order = 1

user_matching_settings_user_matching_setting2_source_identifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting2SourceIdentifier.code = 'username'


userMatchingSettingsUserMatchingSetting2.source_identifier = userMatchingSettingsUserMatchingSetting2SourceIdentifier
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups(\'students\')', 
];
userMatchingSettingsUserMatchingSetting2.additionaldata(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting2;
request_body.usermatchingsettings(userMatchingSettingsArray)





result = await client.external.industryData.sourceSystems.post(request_body = request_body)


```