# ReccitoSdk::ReceiptCreate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **merchant_receipt_id** | **String** |  | [optional] |
| **dedupe_key** | **String** |  | [optional] |
| **barcode** | [**Barcode**](Barcode.md) |  | [optional] |
| **store_id** | **String** |  | [optional] |
| **transaction_date** | **Time** |  |  |
| **order_number** | **String** |  | [optional] |
| **cashier** | **String** |  | [optional] |
| **items** | [**Array&lt;ReceiptItemCreate&gt;**](ReceiptItemCreate.md) |  |  |
| **subtotal** | **String** |  |  |
| **tax_amount** | **String** |  |  |
| **discount_amount** | **String** |  | [optional][default to &#39;0&#39;] |
| **tip_amount** | **String** |  | [optional][default to &#39;0&#39;] |
| **total_amount** | **String** |  |  |
| **currency** | **String** |  |  |
| **payment_info** | [**Array&lt;PaymentInfoCreate&gt;**](PaymentInfoCreate.md) |  |  |
| **notes** | **String** |  | [optional] |
| **return_policy** | **String** |  | [optional] |
| **offers** | **Array&lt;String&gt;** |  | [optional] |
| **offer_policies** | [**Array&lt;OfferPolicyInfo&gt;**](OfferPolicyInfo.md) |  | [optional] |
| **feedback_url** | **String** |  | [optional] |
| **loyalty_info** | **String** |  | [optional] |
| **merchant_details** | [**MerchantDetails**](MerchantDetails.md) |  | [optional] |
| **adjustments** | [**Array&lt;ReceiptAdjustment&gt;**](ReceiptAdjustment.md) |  | [optional] |
| **transaction_references** | [**Array&lt;TransactionReference&gt;**](TransactionReference.md) |  | [optional] |
| **warranties** | [**Array&lt;WarrantyInfo&gt;**](WarrantyInfo.md) |  | [optional] |
| **insights** | [**ReceiptInsights**](ReceiptInsights.md) |  | [optional] |
| **return_insights** | [**ReturnInsights**](ReturnInsights.md) |  | [optional] |
| **qr_expiry_minutes** | **Integer** |  | [optional] |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::ReceiptCreate.new(
  merchant_receipt_id: null,
  dedupe_key: null,
  barcode: null,
  store_id: null,
  transaction_date: null,
  order_number: null,
  cashier: null,
  items: null,
  subtotal: 12.99,
  tax_amount: 12.99,
  discount_amount: 12.99,
  tip_amount: 12.99,
  total_amount: 12.99,
  currency: null,
  payment_info: null,
  notes: null,
  return_policy: null,
  offers: null,
  offer_policies: null,
  feedback_url: null,
  loyalty_info: null,
  merchant_details: null,
  adjustments: null,
  transaction_references: null,
  warranties: null,
  insights: null,
  return_insights: null,
  qr_expiry_minutes: null
)
```

