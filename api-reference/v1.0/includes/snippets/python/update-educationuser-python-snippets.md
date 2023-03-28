---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationUser();
$requestBody.setDisplayName('Rogelio Cazares');

$requestBody.setGivenName('Rogelio');

$requestBody.setMiddleName('Fernando');

$requestBody.setSurname('Cazares');



$requestResult = $graphServiceClient.education().usersById('educationUser-id').patch($requestBody);


```