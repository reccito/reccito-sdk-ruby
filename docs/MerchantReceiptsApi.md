# ReccitoSdk::MerchantReceiptsApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_receipt**](MerchantReceiptsApi.md#create_receipt) | **POST** /api/v1/merchant/receipts | Create Receipt |
| [**get_receipt**](MerchantReceiptsApi.md#get_receipt) | **GET** /api/v1/merchant/receipts/{receipt_id} | Get Receipt |
| [**list_receipts**](MerchantReceiptsApi.md#list_receipts) | **GET** /api/v1/merchant/receipts | List Receipts |
| [**refresh_receipt_qr**](MerchantReceiptsApi.md#refresh_receipt_qr) | **PUT** /api/v1/merchant/receipts/{receipt_id}/refresh-qr | Refresh Qr Code |


## create_receipt

> <ReceiptImmediateResponse> create_receipt(receipt_create)

Create Receipt

Create a new receipt. Synchronous: the receipt is durably persisted before this returns (see ReceiptService.create_receipt_synchronously). A retry with the same dedupe_key returns the original receipt with 200, not an error (idempotent replay, Stripe-style).

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantReceiptsApi.new
receipt_create = ReccitoSdk::ReceiptCreate.new({transaction_date: Time.now, items: [ReccitoSdk::ReceiptItemCreate.new({name: 'name_example', quantity: 37, unit_price: '12.99', total_price: '12.99'})], subtotal: '12.99', tax_amount: '12.99', total_amount: '12.99', currency: 'currency_example', payment_info: [ReccitoSdk::PaymentInfoCreate.new({method: 'method_example', amount: '12.99'})]}) # ReceiptCreate | 

begin
  # Create Receipt
  result = api_instance.create_receipt(receipt_create)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->create_receipt: #{e}"
end
```

#### Using the create_receipt_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReceiptImmediateResponse>, Integer, Hash)> create_receipt_with_http_info(receipt_create)

```ruby
begin
  # Create Receipt
  data, status_code, headers = api_instance.create_receipt_with_http_info(receipt_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReceiptImmediateResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->create_receipt_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **receipt_create** | [**ReceiptCreate**](ReceiptCreate.md) |  |  |

### Return type

[**ReceiptImmediateResponse**](ReceiptImmediateResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_receipt

> <MerchantReceiptResponse> get_receipt(receipt_id)

Get Receipt

Get receipt by ID.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantReceiptsApi.new
receipt_id = 'receipt_id_example' # String | 

begin
  # Get Receipt
  result = api_instance.get_receipt(receipt_id)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->get_receipt: #{e}"
end
```

#### Using the get_receipt_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<MerchantReceiptResponse>, Integer, Hash)> get_receipt_with_http_info(receipt_id)

```ruby
begin
  # Get Receipt
  data, status_code, headers = api_instance.get_receipt_with_http_info(receipt_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <MerchantReceiptResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->get_receipt_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **receipt_id** | **String** |  |  |

### Return type

[**MerchantReceiptResponse**](MerchantReceiptResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_receipts

> <ReceiptListResponse> list_receipts(opts)

List Receipts

List receipts with filters and pagination.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantReceiptsApi.new
opts = {
  page: 56, # Integer | 
  limit: 56, # Integer | 
  store_id: 'store_id_example', # String | 
  status: 'status_example', # String | 
  search: 'search_example', # String | 
  sort_by: 'sort_by_example', # String | 
  sort_order: 'sort_order_example' # String | 
}

begin
  # List Receipts
  result = api_instance.list_receipts(opts)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->list_receipts: #{e}"
end
```

#### Using the list_receipts_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ReceiptListResponse>, Integer, Hash)> list_receipts_with_http_info(opts)

```ruby
begin
  # List Receipts
  data, status_code, headers = api_instance.list_receipts_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ReceiptListResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->list_receipts_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **page** | **Integer** |  | [optional][default to 1] |
| **limit** | **Integer** |  | [optional][default to 50] |
| **store_id** | **String** |  | [optional] |
| **status** | **String** |  | [optional] |
| **search** | **String** |  | [optional] |
| **sort_by** | **String** |  | [optional][default to &#39;created_at&#39;] |
| **sort_order** | **String** |  | [optional][default to &#39;desc&#39;] |

### Return type

[**ReceiptListResponse**](ReceiptListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## refresh_receipt_qr

> <QRRefreshResponse> refresh_receipt_qr(receipt_id)

Refresh Qr Code

Refresh QR code for a receipt.

### Examples

```ruby
require 'time'
require 'reccito_sdk'
# setup authorization
ReccitoSdk.configure do |config|
  # Configure Bearer authorization (API Key): ApiKeyAuth
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = ReccitoSdk::MerchantReceiptsApi.new
receipt_id = 'receipt_id_example' # String | 

begin
  # Refresh Qr Code
  result = api_instance.refresh_receipt_qr(receipt_id)
  p result
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->refresh_receipt_qr: #{e}"
end
```

#### Using the refresh_receipt_qr_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<QRRefreshResponse>, Integer, Hash)> refresh_receipt_qr_with_http_info(receipt_id)

```ruby
begin
  # Refresh Qr Code
  data, status_code, headers = api_instance.refresh_receipt_qr_with_http_info(receipt_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <QRRefreshResponse>
rescue ReccitoSdk::ApiError => e
  puts "Error when calling MerchantReceiptsApi->refresh_receipt_qr_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **receipt_id** | **String** |  |  |

### Return type

[**QRRefreshResponse**](QRRefreshResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

