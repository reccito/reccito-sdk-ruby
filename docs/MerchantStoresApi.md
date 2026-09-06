# ReccitoSdk::MerchantStoresApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_store**](MerchantStoresApi.md#create_store) | **POST** /api/v1/merchant/stores | Create Store |
| [**get_store**](MerchantStoresApi.md#get_store) | **GET** /api/v1/merchant/stores/{store_id} | Get Store |
| [**get_store_stats**](MerchantStoresApi.md#get_store_stats) | **GET** /api/v1/merchant/stores/{store_id}/stats | Get Store Stats |
| [**list_stores**](MerchantStoresApi.md#list_stores) | **GET** /api/v1/merchant/stores | List Stores |
| [**update_store**](MerchantStoresApi.md#update_store) | **PUT** /api/v1/merchant/stores/{store_id} | Update Store |


## create_store

> <StoreResponse> create_store(store_create)

Create Store

Create a new store for the organisation.  **Authentication:** Required (Organisation bearer token)

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantStoresApi.new
store_create = ReccitoSdk::StoreCreate.new({name: 'name_example', code: 'code_example'}) # StoreCreate | 

begin
  # Create Store
  result = api_instance.create_store(store_create)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->create_store: #{e}"
end
```

#### Using the create_store_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreResponse>, Integer, Hash)> create_store_with_http_info(store_create)

```ruby
begin
  # Create Store
  data, status_code, headers = api_instance.create_store_with_http_info(store_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->create_store_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_create** | [**StoreCreate**](StoreCreate.md) |  |  |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_store

> <StoreResponse> get_store(store_id)

Get Store

Get a specific store by ID.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - `store_id`: UUID of the store

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantStoresApi.new
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Store
  result = api_instance.get_store(store_id)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->get_store: #{e}"
end
```

#### Using the get_store_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreResponse>, Integer, Hash)> get_store_with_http_info(store_id)

```ruby
begin
  # Get Store
  data, status_code, headers = api_instance.get_store_with_http_info(store_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->get_store_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_id** | **String** |  |  |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_store_stats

> <StoreStatsResponse> get_store_stats(store_id)

Get Store Stats

Get statistics for a store.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - `store_id`: UUID of the store

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantStoresApi.new
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Get Store Stats
  result = api_instance.get_store_stats(store_id)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->get_store_stats: #{e}"
end
```

#### Using the get_store_stats_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreStatsResponse>, Integer, Hash)> get_store_stats_with_http_info(store_id)

```ruby
begin
  # Get Store Stats
  data, status_code, headers = api_instance.get_store_stats_with_http_info(store_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreStatsResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->get_store_stats_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_id** | **String** |  |  |

### Return type

[**StoreStatsResponse**](StoreStatsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_stores

> <StoreListResponse> list_stores(opts)

List Stores

List all stores for the organisation.  **Authentication:** Required (Organisation bearer token)  **Query Parameters:** - `skip`: Number of stores to skip (default: 0) - `limit`: Number of stores to return (default: 100, max: 1000) - `is_active`: Filter by active status (optional) - `q`: Search by store name/code/city/email/phone (optional)

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantStoresApi.new
opts = {
  skip: 56, # Integer | 
  limit: 56, # Integer | 
  is_active: true, # Boolean | 
  q: 'q_example' # String | 
}

begin
  # List Stores
  result = api_instance.list_stores(opts)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->list_stores: #{e}"
end
```

#### Using the list_stores_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreListResponse>, Integer, Hash)> list_stores_with_http_info(opts)

```ruby
begin
  # List Stores
  data, status_code, headers = api_instance.list_stores_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreListResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->list_stores_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **skip** | **Integer** |  | [optional][default to 0] |
| **limit** | **Integer** |  | [optional][default to 100] |
| **is_active** | **Boolean** |  | [optional] |
| **q** | **String** |  | [optional] |

### Return type

[**StoreListResponse**](StoreListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_store

> <StoreResponse> update_store(store_id, store_update)

Update Store

Update a store.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - `store_id`: UUID of the store  **Request Body:** Updated store fields (all optional)

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantStoresApi.new
store_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 
store_update = ReccitoSdk::StoreUpdate.new # StoreUpdate | 

begin
  # Update Store
  result = api_instance.update_store(store_id, store_update)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->update_store: #{e}"
end
```

#### Using the update_store_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<StoreResponse>, Integer, Hash)> update_store_with_http_info(store_id, store_update)

```ruby
begin
  # Update Store
  data, status_code, headers = api_instance.update_store_with_http_info(store_id, store_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <StoreResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantStoresApi->update_store_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_id** | **String** |  |  |
| **store_update** | [**StoreUpdate**](StoreUpdate.md) |  |  |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

