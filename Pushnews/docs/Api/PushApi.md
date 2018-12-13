# Swagger\Client\PushApi

All URIs are relative to *https://api.pushnews.eu/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pushSend**](PushApi.md#pushSend) | **POST** /push/{siteId} | Send a Push Notification


# **pushSend**
> \Swagger\Client\Model\NotificationApiResponse pushSend($site_id, $body)

Send a Push Notification

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Auth-Token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Auth-Token', 'Bearer');

$apiInstance = new Swagger\Client\Api\PushApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$site_id = "site_id_example"; // string | Site ID
$body = new \Swagger\Client\Model\Notification(); // \Swagger\Client\Model\Notification | Notification object

try {
    $result = $apiInstance->pushSend($site_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PushApi->pushSend: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **site_id** | **string**| Site ID |
 **body** | [**\Swagger\Client\Model\Notification**](../Model/Notification.md)| Notification object |

### Return type

[**\Swagger\Client\Model\NotificationApiResponse**](../Model/NotificationApiResponse.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

