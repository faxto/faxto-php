# Swagger\Client\NumberApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**numbersGet**](NumberApi.md#numbersGet) | **GET** /numbers | 


# **numbersGet**
> numbersGet($api_key, $page)



This API get users numbers.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\NumberApi();
$api_key = "api_key_example"; // string | API Key
$page = "page_example"; // string | Page to display

try {
    $api_instance->numbersGet($api_key, $page);
} catch (Exception $e) {
    echo 'Exception when calling NumberApi->numbersGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **page** | **string**| Page to display | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

