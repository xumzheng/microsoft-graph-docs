---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Team();
requestBody.visibility = TeamVisibilityType.Private;
requestBody.displayName = "Sample Engineering Team";
requestBody.description = "This is a sample engineering team, used to showcase the range of properties supported by this API";
const channel = new Channel();
channel.displayName = "Announcements 📢";
channel.isFavoriteByDefault = true;
channel.description = "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.";
const channel1 = new Channel();
channel1.displayName = "Training 🏋️";
channel1.isFavoriteByDefault = true;
channel1.description = "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.";
const teamstab = new TeamsTab();
teamstab.displayName = "A Pinned Website";
teamstab.configuration = new TeamsTabConfiguration();
teamstab.configuration.contentUrl = "https://docs.microsoft.com/microsoftteams/microsoft-teams";
teamstab.additionalData = {
								 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')"
							 }
const teamstab1 = new TeamsTab();
teamstab1.displayName = "A Pinned YouTube Video";
teamstab1.configuration = new TeamsTabConfiguration();
teamstab1.configuration.contentUrl = "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ";
teamstab1.configuration.websiteUrl = "https://www.youtube.com/watch?v=X8krAMdGvCQ";
teamstab1.additionalData = {
								 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')"
							 }
channel1.tabs = [
						teamstab,
						teamstab1
					]
const channel2 = new Channel();
channel2.displayName = "Planning 📅 ";
channel2.description = "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.";
channel2.isFavoriteByDefault = false;
const channel3 = new Channel();
channel3.displayName = "Issues and Feedback 🐞";
channel3.description = "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.";
requestBody.channels = [
			channel,
			channel1,
			channel2,
			channel3
		]
requestBody.memberSettings = new TeamMemberSettings();
requestBody.memberSettings.allowCreateUpdateChannels = true;
requestBody.memberSettings.allowDeleteChannels = true;
requestBody.memberSettings.allowAddRemoveApps = true;
requestBody.memberSettings.allowCreateUpdateRemoveTabs = true;
requestBody.memberSettings.allowCreateUpdateRemoveConnectors = true;
requestBody.guestSettings = new TeamGuestSettings();
requestBody.guestSettings.allowCreateUpdateChannels = false;
requestBody.guestSettings.allowDeleteChannels = false;
requestBody.funSettings = new TeamFunSettings();
requestBody.funSettings.allowGiphy = true;
requestBody.funSettings.giphyContentRating = GiphyRatingType.Moderate;
requestBody.funSettings.allowStickersAndMemes = true;
requestBody.funSettings.allowCustomMemes = true;
requestBody.messagingSettings = new TeamMessagingSettings();
requestBody.messagingSettings.allowUserEditMessages = true;
requestBody.messagingSettings.allowUserDeleteMessages = true;
requestBody.messagingSettings.allowOwnerDeleteMessages = true;
requestBody.messagingSettings.allowTeamMentions = true;
requestBody.messagingSettings.allowChannelMentions = true;
requestBody.discoverySettings = new TeamDiscoverySettings();
requestBody.discoverySettings.showInTeamsSearchAndSuggestions = true;
const teamsappinstallation = new TeamsAppInstallation();
teamsappinstallation.additionalData = {
					 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
				 }
const teamsappinstallation1 = new TeamsAppInstallation();
teamsappinstallation1.additionalData = {
					 "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
				 }
requestBody.installedApps = [
			teamsappinstallation,
			teamsappinstallation1
		]
requestBody.additionalData = {
		 "template@odata.bind" : "https://graph.microsoft.com/beta/teamsTemplates('standard')"
	 }
const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```