# SwaggerClient-php
For all your azubi data needs!

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Build package: io.swagger.codegen.v3.generators.php.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## Documentation for API Endpoints

All URIs are relative to *https://localhost:8000*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**deleteAzubisDeleteAzubi**](docs/Api/DefaultApi.md#deleteazubisdeleteazubi) | **DELETE** /azubis/{id} | 
*DefaultApi* | [**getAzubisGetAzubi**](docs/Api/DefaultApi.md#getazubisgetazubi) | **GET** /azubis/{id} | 
*DefaultApi* | [**getAzubisGetAzubiList**](docs/Api/DefaultApi.md#getazubisgetazubilist) | **GET** /azubis | 
*DefaultApi* | [**patchAzubisPatchAzubi**](docs/Api/DefaultApi.md#patchazubispatchazubi) | **PATCH** /azubis/{id} | 
*DefaultApi* | [**postAzubisPostAzubi**](docs/Api/DefaultApi.md#postazubispostazubi) | **POST** /azubis | 

## Documentation For Models

 - [Azubi](docs/Model/Azubi.md)
 - [AzubisBody](docs/Model/AzubisBody.md)
 - [AzubisIdBody](docs/Model/AzubisIdBody.md)

## Documentation For Authorization

 All endpoints do not require authorization.


## Author



