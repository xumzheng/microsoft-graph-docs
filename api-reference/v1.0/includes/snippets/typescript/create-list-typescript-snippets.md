---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new List();
requestBody.displayName = "Books";
const columndefinition = new ColumnDefinition();
columndefinition.name = "Author";
columndefinition.text = new TextColumn();
const columndefinition1 = new ColumnDefinition();
columndefinition1.name = "PageCount";
columndefinition1.number = new NumberColumn();
requestBody.columns = [
			columndefinition,
			columndefinition1
		]
requestBody.list = new ListInfo();
requestBody.list.template = "genericList";
const result = async () => {
	await graphServiceClient.sitesById("site-id").lists.post(requestBody);
}


```