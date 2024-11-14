# OpenAPI\Client\ConfigManagerApi

All URIs are relative to https://config-manager.api.gogemini.io, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**configManagerBulkSetConfigs()**](ConfigManagerApi.md#configManagerBulkSetConfigs) | **POST** /configmanager.ConfigManager/BulkSetConfigs | BulkSetConfigs |
| [**configManagerGetConfig()**](ConfigManagerApi.md#configManagerGetConfig) | **POST** /configmanager.ConfigManager/GetConfig | GetConfig |
| [**configManagerGetTenantIdByCode()**](ConfigManagerApi.md#configManagerGetTenantIdByCode) | **POST** /configmanager.ConfigManager/GetTenantIdByCode |  |


## `configManagerBulkSetConfigs()`

```php
configManagerBulkSetConfigs($body): object
```

BulkSetConfigs

Bulk set configs

### Example

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

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\ConfigmanagerBulkSetConfigsRequest**](../Model/ConfigmanagerBulkSetConfigsRequest.md)|  | |

### Return type

**object**

### Authorization

[standardAuthorization](../../README.md#standardAuthorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `configManagerGetConfig()`

```php
configManagerGetConfig($body): \OpenAPI\Client\Model\ConfigmanagerConfigResponse
```

GetConfig

Get a config

### Example

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
$body = new \OpenAPI\Client\Model\ConfigmanagerGetConfigRequest(); // \OpenAPI\Client\Model\ConfigmanagerGetConfigRequest

try {
    $result = $apiInstance->configManagerGetConfig($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConfigManagerApi->configManagerGetConfig: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\ConfigmanagerGetConfigRequest**](../Model/ConfigmanagerGetConfigRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ConfigmanagerConfigResponse**](../Model/ConfigmanagerConfigResponse.md)

### Authorization

[standardAuthorization](../../README.md#standardAuthorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `configManagerGetTenantIdByCode()`

```php
configManagerGetTenantIdByCode($body): \OpenAPI\Client\Model\ConfigmanagerGetTenantIdByCodeResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new OpenAPI\Client\Api\ConfigManagerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\ConfigmanagerGetTenantIdByCodeRequest(); // \OpenAPI\Client\Model\ConfigmanagerGetTenantIdByCodeRequest

try {
    $result = $apiInstance->configManagerGetTenantIdByCode($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConfigManagerApi->configManagerGetTenantIdByCode: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | [**\OpenAPI\Client\Model\ConfigmanagerGetTenantIdByCodeRequest**](../Model/ConfigmanagerGetTenantIdByCodeRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ConfigmanagerGetTenantIdByCodeResponse**](../Model/ConfigmanagerGetTenantIdByCodeResponse.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
