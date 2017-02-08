# Swagger\Client\FilesApi

All URIs are relative to *https://fax.to/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**filesGet**](FilesApi.md#filesGet) | **GET** /files | 
[**filesIdDelete**](FilesApi.md#filesIdDelete) | **DELETE** /files/{id} | 
[**filesPost**](FilesApi.md#filesPost) | **POST** /files | 


# **filesGet**
> filesGet($api_key)



This API lists all the files

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FilesApi();
$api_key = "api_key_example"; // string | API Key

try {
    $api_instance->filesGet($api_key);
} catch (Exception $e) {
    echo 'Exception when calling FilesApi->filesGet: ', $e->getMessage(), PHP_EOL;
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

# **filesIdDelete**
> filesIdDelete($api_key, $id)



This API deletes a single file.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FilesApi();
$api_key = "api_key_example"; // string | API Key
$id = 3.4; // float | id of the file / document

try {
    $api_instance->filesIdDelete($api_key, $id);
} catch (Exception $e) {
    echo 'Exception when calling FilesApi->filesIdDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **id** | **float**| id of the file / document |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **filesPost**
> \Swagger\Client\Model\File filesPost($api_key, $file)



This API allows uploading of a single file.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\FilesApi();
$api_key = "api_key_example"; // string | API Key
$file = "/path/to/file.txt"; // \SplFileObject | PDF file to upload

try {
    $result = $api_instance->filesPost($api_key, $file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling FilesApi->filesPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **api_key** | **string**| API Key |
 **file** | **\SplFileObject**| PDF file to upload |

### Return type

[**\Swagger\Client\Model\File**](../Model/File.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

