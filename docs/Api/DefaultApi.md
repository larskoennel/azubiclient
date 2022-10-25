# Swagger\Client\DefaultApi

All URIs are relative to *https://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteAzubisDeleteAzubi**](DefaultApi.md#deleteazubisdeleteazubi) | **DELETE** /azubis/{id} | 
[**getAzubisGetAzubi**](DefaultApi.md#getazubisgetazubi) | **GET** /azubis/{id} | 
[**getAzubisGetAzubiList**](DefaultApi.md#getazubisgetazubilist) | **GET** /azubis | 
[**patchAzubisPatchAzubi**](DefaultApi.md#patchazubispatchazubi) | **PATCH** /azubis/{id} | 
[**postAzubisPostAzubi**](DefaultApi.md#postazubispostazubi) | **POST** /azubis | 

# **deleteAzubisDeleteAzubi**
> \Swagger\Client\Model\Azubi[] deleteAzubisDeleteAzubi($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->deleteAzubisDeleteAzubi($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->deleteAzubisDeleteAzubi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Azubi[]**](../Model/Azubi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getAzubisGetAzubi**
> \Swagger\Client\Model\Azubi[] getAzubisGetAzubi($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = "id_example"; // string | 

try {
    $result = $apiInstance->getAzubisGetAzubi($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getAzubisGetAzubi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Azubi[]**](../Model/Azubi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getAzubisGetAzubiList**
> \Swagger\Client\Model\Azubi[] getAzubisGetAzubiList()



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->getAzubisGetAzubiList();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getAzubisGetAzubiList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\Azubi[]**](../Model/Azubi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **patchAzubisPatchAzubi**
> \Swagger\Client\Model\Azubi[] patchAzubisPatchAzubi($id, $body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id = "id_example"; // string | 
$body = new \Swagger\Client\Model\AzubisIdBody(); // \Swagger\Client\Model\AzubisIdBody | Input data that you want changed.

try {
    $result = $apiInstance->patchAzubisPatchAzubi($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->patchAzubisPatchAzubi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **body** | [**\Swagger\Client\Model\AzubisIdBody**](../Model/AzubisIdBody.md)| Input data that you want changed. | [optional]

### Return type

[**\Swagger\Client\Model\Azubi[]**](../Model/Azubi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **postAzubisPostAzubi**
> \Swagger\Client\Model\Azubi[] postAzubisPostAzubi($body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\AzubisBody(); // \Swagger\Client\Model\AzubisBody | Input the azubi data

try {
    $result = $apiInstance->postAzubisPostAzubi($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->postAzubisPostAzubi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\AzubisBody**](../Model/AzubisBody.md)| Input the azubi data | [optional]

### Return type

[**\Swagger\Client\Model\Azubi[]**](../Model/Azubi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

