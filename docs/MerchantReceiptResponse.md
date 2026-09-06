# ReccitoSdk::MerchantReceiptResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |
| **public_token** | **String** |  |  |
| **barcode** | [**Barcode**](Barcode.md) |  | [optional] |
| **merchant_receipt_id** | **String** |  | [optional] |
| **merchant_name** | **String** |  | [optional] |
| **merchant_logo** | **String** |  | [optional] |
| **store_id** | **String** |  |  |
| **organisation_id** | **String** |  |  |
| **transaction_date** | **Time** |  |  |
| **order_number** | **String** |  | [optional] |
| **cashier** | **String** |  | [optional] |
| **items** | [**Array&lt;ReceiptItemResponse&gt;**](ReceiptItemResponse.md) |  |  |
| **subtotal** | **String** |  |  |
| **tax_amount** | **String** |  |  |
| **discount_amount** | **String** |  |  |
| **tip_amount** | **String** |  |  |
| **total_amount** | **String** |  |  |
| **currency** | **String** |  |  |
| **payment_info** | [**Array&lt;PaymentInfoResponse&gt;**](PaymentInfoResponse.md) |  |  |
| **qr_code_url** | **String** |  |  |
| **qr_token** | **String** |  |  |
| **qr_expires_at** | **Time** |  |  |
| **receipt_url** | **String** |  |  |
| **pdf_url** | **String** |  | [optional] |
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
| **access_count** | **Integer** |  |  |
| **last_accessed** | **Time** |  | [optional] |
| **status** | **String** |  |  |
| **expires_at** | **Time** |  | [optional] |
| **created_at** | **Time** |  |  |
| **updated_at** | **Time** |  |  |

## Example

```ruby
require 'reccito_sdk'

instance = ReccitoSdk::MerchantReceiptResponse.new(
  id: null,
  public_token: null,
  barcode: null,
  merchant_receipt_id: null,
  merchant_name: null,
  merchant_logo: null,
  store_id: null,
  organisation_id: null,
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
  qr_code_url: null,
  qr_token: null,
  qr_expires_at: null,
  receipt_url: null,
  pdf_url: null,
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
  access_count: null,
  last_accessed: null,
  status: null,
  expires_at: null,
  created_at: null,
  updated_at: null
)
```

