# ReccitoSdk::ReceiptImmediateResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **public_token** | **String** |  |  |
| **barcode** | [**Barcode**](Barcode.md) |  | [optional] |
| **merchant_receipt_id** | **String** |  | [optional] |
| **store_id** | **String** |  |  |
| **organisation_id** | **String** |  |  |
| **qr_code_url** | **String** |  |  |
| **qr_token** | **String** |  |  |
| **qr_expires_at** | **Time** |  |  |
| **receipt_url** | **String** |  |  |
| **transaction_date** | **Time** |  |  |
| **total_amount** | **String** |  |  |
| **currency** | **String** |  |  |
| **processing_status** | **String** |  | [optional][default to &#39;processing&#39;] |
| **created_at** | **Time** |  |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptImmediateResponse.new(
  id: null,
  public_token: null,
  barcode: null,
  merchant_receipt_id: null,
  store_id: null,
  organisation_id: null,
  qr_code_url: null,
  qr_token: null,
  qr_expires_at: null,
  receipt_url: null,
  transaction_date: null,
  total_amount: 12.99,
  currency: null,
  processing_status: null,
  created_at: null
)
```

