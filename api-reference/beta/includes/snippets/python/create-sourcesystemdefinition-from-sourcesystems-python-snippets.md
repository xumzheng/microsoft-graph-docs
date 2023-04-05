---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceSystemDefinition()
request_body.setDisplayName('Rostering source')

userMatchingSettingsUserMatchingSetting1 = UserMatchingSetting()
userMatchingSettingsUserMatchingSetting1MatchTarget = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting1MatchTarget.setCode('userPrincipalName')


userMatchingSettingsUserMatchingSetting1.setMatchTarget($userMatchingSettingsUserMatchingSetting1MatchTarget)
userMatchingSettingsUserMatchingSetting1.setPriorityOrder(0)

userMatchingSettingsUserMatchingSetting1SourceIdentifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting1SourceIdentifier.setCode('username')


userMatchingSettingsUserMatchingSetting1.setSourceIdentifier($userMatchingSettingsUserMatchingSetting1SourceIdentifier)
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups/staff', 
];
userMatchingSettingsUserMatchingSetting1.setAdditionalData(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting1;
userMatchingSettingsUserMatchingSetting2 = UserMatchingSetting()
userMatchingSettingsUserMatchingSetting2MatchTarget = UserMatchTargetReferenceValue()
userMatchingSettingsUserMatchingSetting2MatchTarget.setCode('userPrincipalName')


userMatchingSettingsUserMatchingSetting2.setMatchTarget($userMatchingSettingsUserMatchingSetting2MatchTarget)
userMatchingSettingsUserMatchingSetting2.setPriorityOrder(1)

userMatchingSettingsUserMatchingSetting2SourceIdentifier = IdentifierTypeReferenceValue()
userMatchingSettingsUserMatchingSetting2SourceIdentifier.setCode('username')


userMatchingSettingsUserMatchingSetting2.setSourceIdentifier($userMatchingSettingsUserMatchingSetting2SourceIdentifier)
additionalData = [
'roleGroup@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/roleGroups(\'students\')', 
];
userMatchingSettingsUserMatchingSetting2.setAdditionalData(additionalData)



userMatchingSettingsArray []= userMatchingSettingsUserMatchingSetting2;
request_body.setUserMatchingSettings(userMatchingSettingsArray)




result = await client.external.industryData.sourceSystems.post(request_body)


```