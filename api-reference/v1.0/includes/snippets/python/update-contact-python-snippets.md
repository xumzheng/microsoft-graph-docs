---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Contact();
$homeAddress = new PhysicalAddress();
$homeAddress->setStreet('123 Some street');

$homeAddress->setCity('Seattle');

$homeAddress->setState('WA');

$homeAddress->setPostalCode('98121');


$requestBody->setHomeAddress($homeAddress);
$requestBody->setBirthday(new DateTime('1974-07-22'));



$requestResult = $graphServiceClient->me()->contactsById('contact-id')->patch($requestBody);


```