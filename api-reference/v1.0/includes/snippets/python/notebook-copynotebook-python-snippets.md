---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CopyNotebookPostRequestBody();
$requestBody->setGroupId('groupId-value');

$requestBody->setRenameAs('renameAs-value');



$requestResult = $graphServiceClient->me()->onenote()->notebooksById('notebook-id')->copyNotebook()->post($requestBody);


```