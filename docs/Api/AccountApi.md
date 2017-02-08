# Swagger\Client\AccountApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**balanceGet**](AccountApi.md#balanceGet) | **GET** /balance | 


# **balanceGet**
> balanceGet($api_key)



This API get users balance.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\AccountApi();
$api_key = "api_key_example"; // string | API Key

try {
    $api_instance->balanceGet($api_key);
} catch (Exception $e) {
    echo 'Exception when calling AccountApi->balanceGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

