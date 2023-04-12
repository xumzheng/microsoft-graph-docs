---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let topics = await client.api('/search/topic')
	.version('beta')
	.get();

```