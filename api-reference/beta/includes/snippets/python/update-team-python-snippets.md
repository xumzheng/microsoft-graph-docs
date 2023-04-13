---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.is_membership_limited_to_owners = True

member_settings = TeamMemberSettings()
memberSettings.allow_create_update_channels = True


request_body.member_settings = memberSettings
messaging_settings = TeamMessagingSettings()
messagingSettings.allow_user_edit_messages = True

messagingSettings.allow_user_delete_messages = True


request_body.messaging_settings = messagingSettings
fun_settings = TeamFunSettings()
funSettings.allow_giphy = True

funSettings.GiphyContentRating(GiphyRatingType('strict'))


request_body.fun_settings = funSettings
discovery_settings = TeamDiscoverySettings()
discoverySettings.show_in_teams_search_and_suggestions = True


request_body.discovery_settings = discoverySettings



result = await client.teams_by_id('team-id').patch(request_body = request_body)


```