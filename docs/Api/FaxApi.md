# Swagger\Client\FaxApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**faxDocumentIdCostsGet**](FaxApi.md#faxDocumentIdCostsGet) | **GET** /fax/{document_id}/costs | 
[**faxHistoryGet**](FaxApi.md#faxHistoryGet) | **GET** /fax-history | 
[**faxJobIdStatusGet**](FaxApi.md#faxJobIdStatusGet) | **GET** /fax/{job_id}/status | 
[**faxPost**](FaxApi.md#faxPost) | **POST** /fax | 


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

# **faxHistoryGet**
> faxHistoryGet($api_key, $limit, $page)



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
    $api_instance->faxHistoryGet($api_key, $limit, $page);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->faxHistoryGet: ', $e->getMessage(), PHP_EOL;
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

# **faxPost**
> faxPost($api_key, $fax_number, $document_id, $file, $delete_file)



This API send the fax. When we send fax using API, Fax.to send a POST to the Callback URL you specified in https://fax.to/member/api/live. Fax.to send data POST data with the following information fax_job_id, status and message.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FaxApi();
$api_key = "api_key_example"; // string | API Key
$fax_number = "fax_number_example"; // string | Fax Number
$document_id = 56; // int | Document id. If you want to use existing document you need to specify the document_id
$file = "/path/to/file.txt"; // \SplFileObject | PDF file to upload
$delete_file = 56; // int | Whether to delete file after fax transaction. (put 1 to delete)

try {
    $api_instance->faxPost($api_key, $fax_number, $document_id, $file, $delete_file);
} catch (Exception $e) {
    echo 'Exception when calling FaxApi->faxPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **fax_number** | **string**| Fax Number |
 **document_id** | **int**| Document id. If you want to use existing document you need to specify the document_id | [optional]
 **file** | **\SplFileObject**| PDF file to upload | [optional]
 **delete_file** | **int**| Whether to delete file after fax transaction. (put 1 to delete) | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

