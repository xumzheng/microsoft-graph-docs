---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : B2cIdentityUserFlow = {
	id : "Customer",
	userFlowType : "signUpOrSignIn",
	userFlowTypeVersion : 3,
};

const result = async () => {
	await graphServiceClient.identity.b2cUserFlows.post(requestBody);
}


```