---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Contact();
$requestBody.setGivenName('Pavel');

$requestBody.setSurname('Bansky');

$emailAddressesEmailAddress1 = new EmailAddress();
$emailAddressesEmailAddress1.setAddress('pavelb@fabrikam.onmicrosoft.com');

$emailAddressesEmailAddress1.setName('Pavel Bansky');


$emailAddressesArray []= $emailAddressesEmailAddress1;
$requestBody.setEmailAddresses($emailAddressesArray);


$requestBody.setBusinessPhones(['+1 732 555 0102', ]);



$requestResult = $graphServiceClient.me().contacts().post($requestBody);


```