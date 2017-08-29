# Swagger\Client\PushApi

All URIs are relative to *https://api.pushnews.eu/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pushSend**](PushApi.md#pushSend) | **POST** /push/{siteId} | Send a Push Notification


# **pushSend**
> \Swagger\Client\Model\ApiResponse pushSend($site_id, $body)

Send a Push Notification

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: ApiKeyAuth
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Auth-Token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Auth-Token', 'Bearer');

$api_instance = new Swagger\Client\Api\PushApi();
$site_id = "site_id_example"; // string | Site ID
$body = new \Swagger\Client\Model\Notification(); // \Swagger\Client\Model\Notification | Notification object

try {
    $result = $api_instance->pushSend($site_id, $body);
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
 **body** | [**\Swagger\Client\Model\Notification**](../Model/\Swagger\Client\Model\Notification.md)| Notification object |

### Return type

[**\Swagger\Client\Model\ApiResponse**](../Model/ApiResponse.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

