# Pushnews\Push\PushApi

All URIs are relative to *https://api.pushnews.eu/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pushSend**](PushApi.md#pushSend) | **POST** /push/{siteId} | Send a Push Notification


# **pushSend**
> \Pushnews\Model\ApiResponse pushSend($siteId, $body)

Send a Push Notification

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: ApiKeyAuth
Pushnews\Push\Configuration::getDefaultConfiguration()->setApiKey('X-Auth-Token', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Pushnews\Push\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Auth-Token', 'Bearer');

$api_instance = new Pushnews\Push\Api\PushApi();
$siteId = "siteId_example"; // string | Site ID
$body = new \Pushnews\Model\Notification(); // \Pushnews\Model\Notification | Notification object

try {
    $result = $api_instance->pushSend($siteId, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PushApi->pushSend: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **siteId** | **string**| Site ID |
 **body** | [**\Pushnews\Model\Notification**](../Model/\Pushnews\Model\Notification.md)| Notification object |

### Return type

[**\Pushnews\Model\ApiResponse**](../Model/ApiResponse.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

