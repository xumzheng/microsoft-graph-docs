---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceSystemDefinition()
request_body.displayName = 'Rostering source'

userMatchingSettingsUserMatchingSetting1 = UserMatchingSetting()
userMatchingSettingsUserMatchingSetting1MatchTarget = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting1MatchTarget.code = 'userPrincipalName'


userMatchingSettingsUserMatchingSetting1.matchTarget = userMatchingSettingsUserMatchingSetting1MatchTarget
userMatchingSettingsUserMatchingSetting1.priorityOrder = 0

userMatchingSettingsUserMatchingSetting1SourceIdentifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting1SourceIdentifier.code = 'username'


userMatchingSettingsUserMatchingSetting1.sourceIdentifier = userMatchingSettingsUserMatchingSetting1SourceIdentifier
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups/staff', 
];
userMatchingSettingsUserMatchingSetting1.additionaldata(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting1;
userMatchingSettingsUserMatchingSetting2 = UserMatchingSetting()
userMatchingSettingsUserMatchingSetting2MatchTarget = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting2MatchTarget.code = 'userPrincipalName'


userMatchingSettingsUserMatchingSetting2.matchTarget = userMatchingSettingsUserMatchingSetting2MatchTarget
userMatchingSettingsUserMatchingSetting2.priorityOrder = 1

userMatchingSettingsUserMatchingSetting2SourceIdentifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting2SourceIdentifier.code = 'username'


userMatchingSettingsUserMatchingSetting2.sourceIdentifier = userMatchingSettingsUserMatchingSetting2SourceIdentifier
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups(\'students\')', 
];
userMatchingSettingsUserMatchingSetting2.additionaldata(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting2;
request_body.usermatchingsettings(userMatchingSettingsArray)





result = await client.external.industryData.sourceSystems.post(request_body = request_body)


```