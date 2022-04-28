---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationThread();
requestBody.topic = "New Conversation Thread Topic";
const post = new Post();
post.body = new ItemBody();
post.body.contentType = BodyType.Html;
post.body.content = "this is body content";
const recipient = new Recipient();
recipient.additionalData = {
									 ["name" , "Alex Darrow"],
									 ["address" , "alexd@contoso.com"],
							 }
post.newParticipants = [
						recipient
					]
requestBody.posts = [
			post
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").threads.post(requestBody);
}


```