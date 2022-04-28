---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Conversation();
requestBody.topic = "Does anyone have a second?";
const conversationthread = new ConversationThread();
const post = new Post();
post.body = new ItemBody();
post.body.contentType = BodyType.HTML;
post.body.content = "This is urgent!";
const extension = new Extension();
extension.additionalData = {
											 "@odata.type" : "microsoft.graph.openTypeExtension",
											 "extensionName" : "Com.Contoso.Benefits",
											 "companyName" : "Contoso",
											 "expirationDate" : "2016-08-03T11:00:00.000Z",
											 "topPicks" : [
													"Employees only",
													"Add spouse or guest",
													"Add family"
												]
										 }
post.extensions = [
									extension
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