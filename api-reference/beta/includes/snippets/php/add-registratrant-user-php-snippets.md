---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new MeetingRegistrantBase();
$requestBody->set@odatatype('#microsoft.graph.meetingRegistrant');

$additionalData = [
		'firstName' => 'Frederick', 
		'lastName' => 'Cormier', 
		'email' => 'frederick.cormier@contoso.com', 
		'customQuestionAnswers' => $customQuestionAnswers1 = new ();
$		customQuestionAnswers1->setQuestionId('MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=');

$		customQuestionAnswers1->setValue('No');


$customQuestionAnswersArray []= $customQuestionAnswers1;
$customQuestionAnswers2 = new ();
$		customQuestionAnswers2->setQuestionId('MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=');

$		customQuestionAnswers2->setValue('Internet');


$customQuestionAnswersArray []= $customQuestionAnswers2;
$requestBody->setCustomQuestionAnswers($customQuestionAnswersArray);


];
$requestBody->setAdditionalData($additionalData);




$result = $graphServiceClient->usersById('user-id')->onlineMeetingsById('onlineMeeting-id')->registration()->registrants()->post($requestBody);


```