# Sodlapp API Identity

Sodlapp API allows you to Identity, verify and retrieve CIVIL SERVANT'S key information like Employee Name, Sub Organization, Phone Number, Staff ID etc for authorized application.

####################################################################################
 
```php
curl -X GET https://api.sodlapp.com/ippis/xxxxxx -H 
"Authorization: Bearer sk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxx" 
```
##  This will be your Ippis ID, staff ID or phone number
```php
 https://api.sodlapp.com/ippis/xxxxxx 
 ///xxxxxx will be your Ippis ID, staff ID or phone number
```
## This will be your secret token, create one by signing up ( www.developer.sodlapp.com )

```php
 "Authorization: Bearer sk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxx" 
 /// This will be your secret token, create one by signing up
```

## API request example to api.sodlapp.com using the HTTP GET method

An example of making an HTTP GET request to the 
https://api.sodlapp.com/ippis/xxxxxx API endpoint.

``` php

<?php  
$url = "https://api.sodlapp.com/ippis/xxxxxx"; ///xxxxxx will be your Ippis ID, staff ID or phone number
$curl = curl_init($url);
curl_setopt($curl, CURLOPT_URL, $url);
curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);

$headers = array(
    'Accept: application/json',
    'Content-Type: application/x-www-form-urlencoded',
    'Authorization: Bearer sk_live_xxxxxxxxxxxxxxxxxxxxxx', // this will be your secret token, create one by signing up
);

curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);
//for debug only!
curl_setopt($curl, CURLOPT_SSL_VERIFYHOST, false);
curl_setopt($curl, CURLOPT_SSL_VERIFYPEER, false);

$resp = curl_exec($curl);
curl_close($curl);
 
print_r($resp); // all json fields


?>
```
Visit Sodlapp website www.sodlapp.com

						
