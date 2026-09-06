# ReccitoSdk::StoreStatsResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **store_id** | **String** |  |  |
| **store_name** | **String** |  |  |
| **receipts_created_count** | **Integer** |  |  |
| **receipts_created_today** | **Integer** |  |  |
| **receipts_created_this_month** | **Integer** |  |  |
| **qr_scans_count** | **Integer** |  |  |
| **qr_scans_today** | **Integer** |  |  |
| **qr_scans_this_month** | **Integer** |  |  |
| **total_amount_this_month** | **String** |  |  |
| **average_receipt_amount** | **String** |  |  |
| **last_receipt_created** | **Time** |  | [optional] |
| **busiest_hour** | **String** |  | [optional] |
| **busiest_day** | **String** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::StoreStatsResponse.new(
  store_id: null,
  store_name: null,
  receipts_created_count: null,
  receipts_created_today: null,
  receipts_created_this_month: null,
  qr_scans_count: null,
  qr_scans_today: null,
  qr_scans_this_month: null,
  total_amount_this_month: null,
  average_receipt_amount: null,
  last_receipt_created: null,
  busiest_hour: null,
  busiest_day: null
)
```

