# GeminiCommerce\Configmanager\ConfigManagerApi

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
$config = GeminiCommerce\Configmanager\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new GeminiCommerce\Configmanager\Api\ConfigManagerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Configmanager\Model\ConfigmanagerBulkSetConfigsRequest(); // \GeminiCommerce\Configmanager\Model\ConfigmanagerBulkSetConfigsRequest

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
| **body** | [**\GeminiCommerce\Configmanager\Model\ConfigmanagerBulkSetConfigsRequest**](../Model/ConfigmanagerBulkSetConfigsRequest.md)|  | |

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
configManagerGetConfig($body): \GeminiCommerce\Configmanager\Model\ConfigmanagerConfigResponse
```

GetConfig

Get a config

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure OAuth2 access token for authorization: standardAuthorization
$config = GeminiCommerce\Configmanager\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new GeminiCommerce\Configmanager\Api\ConfigManagerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Configmanager\Model\ConfigmanagerGetConfigRequest(); // \GeminiCommerce\Configmanager\Model\ConfigmanagerGetConfigRequest

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
| **body** | [**\GeminiCommerce\Configmanager\Model\ConfigmanagerGetConfigRequest**](../Model/ConfigmanagerGetConfigRequest.md)|  | |

### Return type

[**\GeminiCommerce\Configmanager\Model\ConfigmanagerConfigResponse**](../Model/ConfigmanagerConfigResponse.md)

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
configManagerGetTenantIdByCode($body): \GeminiCommerce\Configmanager\Model\ConfigmanagerGetTenantIdByCodeResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: Authorization
$config = GeminiCommerce\Configmanager\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = GeminiCommerce\Configmanager\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new GeminiCommerce\Configmanager\Api\ConfigManagerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \GeminiCommerce\Configmanager\Model\ConfigmanagerGetTenantIdByCodeRequest(); // \GeminiCommerce\Configmanager\Model\ConfigmanagerGetTenantIdByCodeRequest

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
| **body** | [**\GeminiCommerce\Configmanager\Model\ConfigmanagerGetTenantIdByCodeRequest**](../Model/ConfigmanagerGetTenantIdByCodeRequest.md)|  | |

### Return type

[**\GeminiCommerce\Configmanager\Model\ConfigmanagerGetTenantIdByCodeResponse**](../Model/ConfigmanagerGetTenantIdByCodeResponse.md)

### Authorization

[Authorization](../../README.md#Authorization)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
