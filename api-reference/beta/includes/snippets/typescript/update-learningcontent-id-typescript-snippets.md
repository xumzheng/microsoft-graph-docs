---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LearningContent = {
	title : "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
	description : "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
	contentWebUrl : "https://learn.microsoft.com/learn/modules/manage-classes-resources-assessment-planning-beedle/",
	sourceName : "MsLearn",
	thumbnailWebUrl : "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
	languageTag : "en-us",
	numberOfPages : 9,
	duration : pT20M,
	format : "Book",
	createdDateTime : new Date("2018-01-01T00:00:00Z"),
	lastModifiedDateTime : new Date("2021-04-01T04:26:06.1995367Z"),
	contributors : [
		"Scott Simpson",
	],
	additionalTags : [
		"Create private or public teams",
		"Add members to teams",
	],
	skillTags : [
		"Create teams",
		"Teams channels",
		"Teams members",
	],
	isActive : true,
	isPremium : false,
	isSearchable : true,
};

const result = async () => {
	await graphServiceClient.employeeExperience.learningProvidersById("learningProvider-id").learningContentsById("learningContent-id").patch(requestBody);
}


```