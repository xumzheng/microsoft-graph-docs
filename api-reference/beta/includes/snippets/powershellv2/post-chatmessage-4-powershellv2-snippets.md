---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Teams

$params = @{
	Body = @{
		ContentType = "html"
		Content = "Here's the latest budget. <attachment id="153fa47d-18c9-4179-be08-9879815a9f90"></attachment>"
	}
	Attachments = @(
		@{
			Id = "153fa47d-18c9-4179-be08-9879815a9f90"
			ContentType = "reference"
			ContentUrl = "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx"
			Name = "Budget.docx"
		}
	)
}

New-MgBetaTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```