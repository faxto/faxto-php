# Swagger\Client\FaxApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**faxDocumentIdCostsGet**](FaxApi.md#faxDocumentIdCostsGet) | **GET** /fax/{document_id}/costs | 
[**faxGet**](FaxApi.md#faxGet) | **GET** /fax | 
[**faxJobIdStatusGet**](FaxApi.md#faxJobIdStatusGet) | **GET** /fax/{job_id}/status | 
[**incomingFaxesGet**](FaxApi.md#incomingFaxesGet) | **GET** /incoming-faxes | 
[**incomingFaxesNumberGet**](FaxApi.md#incomingFaxesNumberGet) | **GET** /incoming-faxes/{number} | 
[**provisionNumbersGet**](FaxApi.md#provisionNumbersGet) | **GET** /provision-numbers | 


# **faxDocumentIdCostsGet**
> faxDocumentIdCostsGet($api_key, $fax_number, $document_id)



This API get the cost of a sending fax.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$fax_number = "fax_number_example"; // string | Fax Number
$document_id = 3.4; // float | id of the file / document_id

try {
    $api_instance->faxDocumentIdCostsGet($api_key, $fax_number, $document_id);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->faxDocumentIdCostsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **fax_number** | **string**| Fax Number |
 **document_id** | **float**| id of the file / document_id |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **faxGet**
> faxGet($api_key, $limit, $page)



This API get all fax history.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$limit = "limit_example"; // string | Number of records to return
$page = "page_example"; // string | Page to display

try {
    $api_instance->faxGet($api_key, $limit, $page);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->faxGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **limit** | **string**| Number of records to return | [optional]
 **page** | **string**| Page to display | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **faxJobIdStatusGet**
> faxJobIdStatusGet($api_key, $job_id)



This API get the status of the fax.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$job_id = 3.4; // float | id of the fax job

try {
    $api_instance->faxJobIdStatusGet($api_key, $job_id);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->faxJobIdStatusGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **job_id** | **float**| id of the fax job |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **incomingFaxesGet**
> incomingFaxesGet($api_key)



This API get faxes .

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key

try {
    $api_instance->incomingFaxesGet($api_key);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->incomingFaxesGet: ', $e->getMessage(), PHP_EOL;
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

# **incomingFaxesNumberGet**
> incomingFaxesNumberGet($api_key, $number)



This API get faxes  by number.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$number = "number_example"; // string | Number in the fax

try {
    $api_instance->incomingFaxesNumberGet($api_key, $number);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->incomingFaxesNumberGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **number** | **string**| Number in the fax |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **provisionNumbersGet**
> provisionNumbersGet($api_key, $limit)



This API get Provision numbers.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$limit = "limit_example"; // string | Limit to display

try {
    $api_instance->provisionNumbersGet($api_key, $limit);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->provisionNumbersGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **limit** | **string**| Limit to display | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

