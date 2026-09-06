# ReccitoSdk::MerchantAssetsApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**list_organisation_assets**](MerchantAssetsApi.md#list_organisation_assets) | **GET** /api/v1/merchant/assets/list | List organisation assets |
| [**upload_organisation_banner**](MerchantAssetsApi.md#upload_organisation_banner) | **POST** /api/v1/merchant/assets/upload/banner | Upload organisation banner |
| [**upload_organisation_logo**](MerchantAssetsApi.md#upload_organisation_logo) | **POST** /api/v1/merchant/assets/upload/logo | Upload organisation logo |
| [**upload_store_logo**](MerchantAssetsApi.md#upload_store_logo) | **POST** /api/v1/merchant/assets/upload/store/logo | Upload store logo |


## list_organisation_assets

> <ApiResponse> list_organisation_assets(opts)

List organisation assets

List all branding assets uploaded for the organisation.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantAssetsApi.new
opts = {
  asset_type: 'asset_type_example' # String | 
}

begin
  # List organisation assets
  result = api_instance.list_organisation_assets(opts)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->list_organisation_assets: #{e}"
end
```

#### Using the list_organisation_assets_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApiResponse>, Integer, Hash)> list_organisation_assets_with_http_info(opts)

```ruby
begin
  # List organisation assets
  data, status_code, headers = api_instance.list_organisation_assets_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApiResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->list_organisation_assets_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **asset_type** | **String** |  | [optional] |

### Return type

[**ApiResponse**](ApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## upload_organisation_banner

> <ApiResponse> upload_organisation_banner(file)

Upload organisation banner

Upload a banner file for the organisation. Supported formats: JPEG, PNG, WebP. Max 5MB.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantAssetsApi.new
file = File.new('/path/to/some/file') # File | Banner file to upload

begin
  # Upload organisation banner
  result = api_instance.upload_organisation_banner(file)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_organisation_banner: #{e}"
end
```

#### Using the upload_organisation_banner_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApiResponse>, Integer, Hash)> upload_organisation_banner_with_http_info(file)

```ruby
begin
  # Upload organisation banner
  data, status_code, headers = api_instance.upload_organisation_banner_with_http_info(file)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApiResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_organisation_banner_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file** | **File** | Banner file to upload |  |

### Return type

[**ApiResponse**](ApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## upload_organisation_logo

> <ApiResponse> upload_organisation_logo(file)

Upload organisation logo

Upload a logo file for the organisation. Supported formats: JPEG, PNG, WebP, SVG. Max 5MB.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantAssetsApi.new
file = File.new('/path/to/some/file') # File | Logo file to upload

begin
  # Upload organisation logo
  result = api_instance.upload_organisation_logo(file)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_organisation_logo: #{e}"
end
```

#### Using the upload_organisation_logo_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApiResponse>, Integer, Hash)> upload_organisation_logo_with_http_info(file)

```ruby
begin
  # Upload organisation logo
  data, status_code, headers = api_instance.upload_organisation_logo_with_http_info(file)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApiResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_organisation_logo_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file** | **File** | Logo file to upload |  |

### Return type

[**ApiResponse**](ApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## upload_store_logo

> <ApiResponse> upload_store_logo(store_id, file)

Upload store logo

Upload a logo file for a specific store. Supported formats: JPEG, PNG, WebP, SVG. Max 5MB.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantAssetsApi.new
store_id = 'store_id_example' # String | 
file = File.new('/path/to/some/file') # File | Store logo file to upload

begin
  # Upload store logo
  result = api_instance.upload_store_logo(store_id, file)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_store_logo: #{e}"
end
```

#### Using the upload_store_logo_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApiResponse>, Integer, Hash)> upload_store_logo_with_http_info(store_id, file)

```ruby
begin
  # Upload store logo
  data, status_code, headers = api_instance.upload_store_logo_with_http_info(store_id, file)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApiResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantAssetsApi->upload_store_logo_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_id** | **String** |  |  |
| **file** | **File** | Store logo file to upload |  |

### Return type

[**ApiResponse**](ApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

