# Swagger\Client\CountryApi

All URIs are relative to *https://fax.to/api/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**areacodesCountryCodeStateIdGet**](CountryApi.md#areacodesCountryCodeStateIdGet) | **GET** /areacodes/{countryCode}/{stateId} | 
[**countriesCountryCodeDidgroupsGet**](CountryApi.md#countriesCountryCodeDidgroupsGet) | **GET** /countries/{countryCode}/didgroups | 
[**countriesDidgroupsDidGroupIdProvisionPost**](CountryApi.md#countriesDidgroupsDidGroupIdProvisionPost) | **POST** /countries/didgroups/{didGroupId}/provision | 
[**countriesGet**](CountryApi.md#countriesGet) | **GET** /countries | 
[**statesCountryCodeGet**](CountryApi.md#statesCountryCodeGet) | **GET** /states/{countryCode} | 


# **areacodesCountryCodeStateIdGet**
> areacodesCountryCodeStateIdGet($country_code, $state_id)



This API get areacodes .

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CountryApi();
$country_code = "country_code_example"; // string | countryCode in the Country
$state_id = "state_id_example"; // string | stateId in the Country

try {
    $api_instance->areacodesCountryCodeStateIdGet($country_code, $state_id);
} catch (Exception $e) {
    echo 'Exception when calling CountryApi->areacodesCountryCodeStateIdGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **string**| countryCode in the Country |
 **state_id** | **string**| stateId in the Country |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **countriesCountryCodeDidgroupsGet**
> countriesCountryCodeDidgroupsGet($country_code, $did_group_ids, $state_id, $city_name_pattern)



This API didgroups countryCode.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CountryApi();
$country_code = "country_code_example"; // string | countryCode in the Country
$did_group_ids = "did_group_ids_example"; // string | didGroupId in the Country
$state_id = "state_id_example"; // string | stateId in the Country
$city_name_pattern = "city_name_pattern_example"; // string | cityNamePattern in the Country

try {
    $api_instance->countriesCountryCodeDidgroupsGet($country_code, $did_group_ids, $state_id, $city_name_pattern);
} catch (Exception $e) {
    echo 'Exception when calling CountryApi->countriesCountryCodeDidgroupsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **string**| countryCode in the Country |
 **did_group_ids** | **string**| didGroupId in the Country |
 **state_id** | **string**| stateId in the Country |
 **city_name_pattern** | **string**| cityNamePattern in the Country |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **countriesDidgroupsDidGroupIdProvisionPost**
> countriesDidgroupsDidGroupIdProvisionPost($did_group_id)



This API didgroups provision.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CountryApi();
$did_group_id = "did_group_id_example"; // string | didGroupId in the Country

try {
    $api_instance->countriesDidgroupsDidGroupIdProvisionPost($did_group_id);
} catch (Exception $e) {
    echo 'Exception when calling CountryApi->countriesDidgroupsDidGroupIdProvisionPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **did_group_id** | **string**| didGroupId in the Country |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **countriesGet**
> countriesGet()



This API get countries.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CountryApi();

try {
    $api_instance->countriesGet();
} catch (Exception $e) {
    echo 'Exception when calling CountryApi->countriesGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **statesCountryCodeGet**
> statesCountryCodeGet($country_code)



This API get States .

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CountryApi();
$country_code = "country_code_example"; // string | countryCode in the Country

try {
    $api_instance->statesCountryCodeGet($country_code);
} catch (Exception $e) {
    echo 'Exception when calling CountryApi->statesCountryCodeGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_code** | **string**| countryCode in the Country |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

