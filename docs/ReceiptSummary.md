# ReccitoSdk::ReceiptSummary

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **public_token** | **String** |  |  |
| **merchant_receipt_id** | **String** |  | [optional] |
| **store_id** | **String** |  |  |
| **organisation_id** | **String** |  |  |
| **transaction_date** | **Time** |  |  |
| **total_amount** | **String** |  |  |
| **currency** | **String** |  |  |
| **item_count** | **Integer** |  |  |
| **status** | **String** |  |  |
| **access_count** | **Integer** |  |  |
| **receipt_url** | **String** |  |  |
| **created_at** | **Time** |  |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptSummary.new(
  id: null,
  public_token: null,
  merchant_receipt_id: null,
  store_id: null,
  organisation_id: null,
  transaction_date: null,
  total_amount: 12.99,
  currency: null,
  item_count: null,
  status: null,
  access_count: null,
  receipt_url: null,
  created_at: null
)
```

