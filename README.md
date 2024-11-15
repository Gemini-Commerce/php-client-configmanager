# configmanager

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)


## Installation & Usage

### Requirements

PHP 7.4 and later.
Should also work with PHP 8.0.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/Gemini-Commerce/php-client-configmanager.git"
    }
  ],
  "require": {
    "Gemini-Commerce/php-client-configmanager": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/configmanager/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



// Configure OAuth2 access token for authorization: standardAuthorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ConfigManagerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\ConfigmanagerBulkSetConfigsRequest(); // \OpenAPI\Client\Model\ConfigmanagerBulkSetConfigsRequest

try {
    $result = $apiInstance->configManagerBulkSetConfigs($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConfigManagerApi->configManagerBulkSetConfigs: ', $e->getMessage(), PHP_EOL;
}

```

## API Endpoints

All URIs are relative to *https://config-manager.api.gogemini.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ConfigManagerApi* | [**configManagerBulkSetConfigs**](docs/Api/ConfigManagerApi.md#configmanagerbulksetconfigs) | **POST** /configmanager.ConfigManager/BulkSetConfigs | BulkSetConfigs
*ConfigManagerApi* | [**configManagerGetConfig**](docs/Api/ConfigManagerApi.md#configmanagergetconfig) | **POST** /configmanager.ConfigManager/GetConfig | GetConfig
*ConfigManagerApi* | [**configManagerGetTenantIdByCode**](docs/Api/ConfigManagerApi.md#configmanagergettenantidbycode) | **POST** /configmanager.ConfigManager/GetTenantIdByCode | 

## Models

- [BulkSetConfigsRequestConfig](docs/Model/BulkSetConfigsRequestConfig.md)
- [ConfigmanagerBulkSetConfigsRequest](docs/Model/ConfigmanagerBulkSetConfigsRequest.md)
- [ConfigmanagerConfigResponse](docs/Model/ConfigmanagerConfigResponse.md)
- [ConfigmanagerGetConfigRequest](docs/Model/ConfigmanagerGetConfigRequest.md)
- [ConfigmanagerGetTenantIdByCodeRequest](docs/Model/ConfigmanagerGetTenantIdByCodeRequest.md)
- [ConfigmanagerGetTenantIdByCodeResponse](docs/Model/ConfigmanagerGetTenantIdByCodeResponse.md)
- [ProtobufAny](docs/Model/ProtobufAny.md)
- [RpcStatus](docs/Model/RpcStatus.md)

## Authorization

Authentication schemes defined for the API:
### Authorization

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


### standardAuthorization

- **Type**: `OAuth`
- **Flow**: `implicit`
- **Authorization URL**: ``
- **Scopes**: N/A

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author

info@gemini-commerce.com

## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.0.0`
    - Generator version: `7.9.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
