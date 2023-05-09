---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LearningProvider = {
	displayName : "Microsoft",
	squareLogoWebUrlForDarkTheme : "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
	longLogoWebUrlForDarkTheme : "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
	squareLogoWebUrlForLightTheme : "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
	longLogoWebUrlForLightTheme : "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
	loginWebUrl : "https://www.linkedin.com/learning-login/teams",
	additionalData : {
		isEnabled : false,
	},
};

const result = async () => {
	await graphServiceClient.employeeExperience.learningProvidersById("learningProvider-id").patch(requestBody);
}


```