---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Conversation();
requestBody.topic = "Take your wellness days and rest";
const conversationthread = new ConversationThread();
const post = new Post();
post.body = new ItemBody();
post.body.contentType = BodyType.Html;
post.body.content = "Contoso cares about you: Rest and Recharge";
const recipient = new Recipient();
recipient.additionalData = {
												 ["name" , "Adele Vance"],
												 ["address" , "AdeleV@contoso.onmicrosoft.com"],
										 }
post.newParticipants = [
									recipient
								]
conversationthread.posts = [
						post
					]
requestBody.threads = [
			conversationthread
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").conversations.post(requestBody);
}


```