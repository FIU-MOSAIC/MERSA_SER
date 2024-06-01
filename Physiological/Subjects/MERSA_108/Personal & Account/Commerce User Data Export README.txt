Commerce User Data Export

This portion of your data export includes data on your orders placed

User Orders.csv:
---------
      confirmation_number                    - String uniquely identifying the order. Customer can refer to the order by this string
      order_status                           - Current status of the order
      store_code                             - Store from which the order was purchased
      checkout_date                          - Date when the order was placed
      customer_email                         - User email that is filled in the address info on checkout for the order
      customer_phone                         - User phone that is filled in the address info on checkout for the order
      billing_address.name                   - Full name of the user filled for billing address
      billing_address.company                - Company name filled for billing address
      billing_address.address1               - Address line 1 for the billing address
      billing_address.address2               - Address line 2 for the billing address
      billing_address.city                   - City filled in the billing address
      billing_address.state                  - State filled in the billing address
      billing_address.postal                 - Postal code filled in the billing address
      billing_address.phone                  - Phone filled in the billing address
      shipping_address.name                  - Full name of the user filled for the shipping address
      shipping_address.company               - Company name filled for the shipping address
      shipping_address.address1              - Address line 1 for the shipping address
      shipping_address.address2              - Address line 2 for the shipping address
      shipping_address.city                  - City filled in the shipping address
      shipping_address.state                 - State filled in the shipping address
      shipping_address.postal                - Postal code filled in the shipping address
      shipping_address.phone                 - Phone filled in the shipping address
      currency_code                          - Currency in which the order was paid
      promo_code                             - Promo code applied for discount in the order
      user_promo_code                        - An individual user promo code in the order applied for discount
      total_shipping_cost                    - Total shipping cost for the order
      total_shipping_cost_override           - Whether total shipping cost is overridden
      estimated_shipping_tax                 - Estimation for tax on shipping
      locale_language                        - Appropriate language for the country selected as a region on fitbit.com, affects in which language the user sees pages during checkout
      locale_country                         - Country selected as a region on fitbit.com
      tax_exempt                             - Whether the order is free from taxes
      case_number                            - A number in case it is placed by CS via Admin Tool for example as replacement order, if applicable
      pre_tax_shipping_cost                  - Shipping cost for the order before tax
      ip_address                             - Ip address the order is placed from
      order_line_item.sku_code               - SKU code of the current item in the line of the order
      order_line_item.unit_price             - Unit price of one item in the current line
      order_line_item.unit_count             - Number of units in the current line
      order_line_item.estimated_tax_per_unit - Tax per each item in the current line
      order_line_item.estimated_tax          - Tax for the current line
      order_line_item.transmitted_count      - Number of units transmitted to warehouse but not shipped yet for the current line
      order_line_item.shipped_count          - Number of units shipped already to the user for the current line
      order_line_item.full_unit_price        - The full price for the current line (line can contain 1 or more units)
      order_line_item.promo_applied          - Whether promo is applied for the current line
      order_line_item.pre_tax_unit_price     - Unit price before tax

User Order Gift Options.csv:
---------
      order.confirmation_number              - Appropriate order confirmation number
      gift_message_sending_method            - When to send the gift to the recipient
      recipient_email                        - Email of the recipient
      sender_name                            - Name of the sender
      recipient_name                         - Name of the recipient
      custom_message                         - Custom message if provided
      gift_message_send_date                 - Date of the gift message sending

User Fulfillments.csv:
---------
      order.confirmation_number                - Order confirmation number
      fulfillment_status                       - Current status of the fulfillment
      warehouse_transmit_date                  - Date when the fulfillment is transmitted to warehouse for shipping
      warehouse_accept_reject_date             - Date when the transmitted fulfillment was accepted or rejected by the warehouse
      shipping_tax_due                         - Required shipping tax for the fulfillment
      shipping_tax_charged                     - Actual charged amount of the tax charged for the fulfillment
      customer_email                           - Email of the customer for the current fulfillment
      shipping_cost                            - Overall shipping cost for the current fulfillment
      scac                                     - SCAC(Standard Carrier Alpha Code) for the current fulfillment
      created_date                             - When the fulfillment is created
      completed_date                           - When the fulfillment can be considered as completed (shipped or provided)
      pre_tax_shipping_cost                    - Tax shipping cost before tax
      fulfillment_line_item.sku_code           - SKU code of the current item in the fulfillment
      fulfillment_line_item.unit_price         - Price of one unit in the line
      fulfillment_line_item.unit_count         - Count of units in the line
      fulfillment_line_item.transmitted_count  - Number of units transmitted to the warehouse for shipping
      fulfillment_line_item.shipped_count      - Number of units shipped by the warehouse
      fulfillment_line_item.tax_due            - Required tax for the current line
      fulfillment_line_item.tax_charged        - Actual charged amount of tax for the current line
      fulfillment_line_item.pre_tax_unit_price - Price of one unit in the line
      package_tracking.tracking_number         - Tracking number of the package for the fulfillment
      package_tracking.carrier                 - Carrier of the package for the fulfillment
      package_tracking.ship_date               - Ship date of the package for the fulfillment
      package_tracking.basic_tracking_url      - Tracking url for the package
      package_tracking.narvar_tracking_url     - Tracking url for the package in Narvar system

User Order Payments.csv:
---------
      order.confirmation_number                - Order confirmation number
      processor_code                           - Processor code identifying who processed the payment (DIGITALRIVER, STRIPE, COMP, PAYPAL_US, PAYPAL_CA)
      payment_processor_validate_ref_id        - Token identifying the current validation of the payment
      processor_validate_date                  - Date of the validation
      authorization_status                     - Either complimentary if payment is not required or validated if some payment method is selected
      card_type                                - Type of card used for the payment
      card_number_suffix                       - Last 4 digits of the card used for the payment
      card_expiration_month                    - Card Expiration month of the card used for the payment
      card_expiration_year                     - Card Expiration year of the card used for the payment
      transaction_type                         - Type of the current transaction. Identifies its intention. Can be payment, refund, complimentary
      transaction_date                         - Date of the latest transaction operation. Operations can be auth, sale, capture, refund
      payment_processor_sale_ref_id            - Token of the appropriate sale (authorization + capture at once) operation if it occured in the scope of the current payment flow
      payment_processor_sale_date              - Date of the sale operation
      payment_amount                           - Payment Amount for the current payment, how much it captures, refunds or sales
      payment_processor_refund_ref_id          - Token of the appropriate refund operation if it occurred in the scope of the current payment flow
      payment_processor_refund_date            - Date of the refund operation
      payment_processor_authorization_ref_id   - Token of the appropriate authorization operation (authorizes that the payment source has enough money, blocking it but not capturing) if it occurred in the scope of the current payment flow
      payment_processor_authorization_date     - Date of the authorization operation
      authorization_amount                     - Authorization amount (how much money it authorized to charge) for the current payment
      payment_processor_capture_ref_id         - Token of the appropriate capture operation (charges money from the payment source) if it occurred in the scope of the current payment flow
      payment_processor_capture_date           - Date of the capture operation

User Order Payment Disputes.csv:
---------
      order.confirmation_number                - Order confirmation number
      chargeback_id                            - Token identifying the dispute
      charge_id                                - Token of the appropriate charge(capture) that was disputed
      create_date                              - Date when the dispute was created
      due_date                                 - Date by which evidence must be submitted in order to successfully challenge dispute
      disputed_amount                          - Disputed amount out of the full charge. Usually the amount of the charge but can differ
      currency_code                            - Currency code
      status                                   - Current status of the dispute
      reason                                   - Reason given by cardholder for dispute
      is_refundable                            - If true it is still possible to refund the disputed payment
      settlement_type                          - Applicable only in case of PayPal disputes

User Order Transaction Logs.csv:
---------
      order.confirmation_number                - Order confirmation number
      transaction_date                         - Date of the appropriate payment transaction
      raw_request                              - Raw string containing info, on type of the transaction operation, payment processor, input token or any other meta data required by the payment processor to make a transaction operation, may contain user data if that is required by the processor
      raw_response                             - Raw response received by a payment processor, contains token, description of the transaction and other data identifying the transaction. Can be encoded as raw comma-separated string or json depending on the payment processor
      response_code                            - Response code describing if the current transaction was successful or not. 100 is success, 400 is error
      amount                                   - Amount of the current transaction

User Subscription Transactions.csv:
---------
      order.confirmation_number                - Order confirmation number
      date_charged                             - Date when money is charged for the current transaction
      amount_charged                           - Charged amount in the scope of the current transaction
      total_amount                             - Total amount to be charged
      payment_processor_ref_id                 - Token identifying the current transaction
      tax_amount                               - Tax amount
      currency                                 - Currency which transaction is paid in

User Refunds.csv:
---------
      order.confirmation_number                - Appropriate Order confirmation number
      refund_date                              - Date of the refund
      refund_amount                            - Full amount of the refund
      refund_tax_component                     - Tax part in the refunded amount
      refund_shipping_component                - Shipping part in the refunded amount
      refund_merchandise_component             - Merchandise part in the refunded amount
      comments                                 - Comments on reason of the refund
      refund_line_item.serial_number           - Serial number of the device this refund is applied to
      refund_line_item.sku                     - SKU of the refunded item
      refund_line_item.unit_refund_amount      - Refund amount of the current line out of the full refund
      refund_line_item.unit_count              - Number of units in the line of the refund
      refund_line_item.tax_refunded            - Tax part of the current line

User Returns.csv:
---------
      order.confirmation_number                - Appropriate Order confirmation number
      case_number                              - An unique number which this return can be referred to by, if provided
      customer_email                           - Email of the user this return is for
      authorize_date                           - Date of the authorization for the current return
      return_reason                            - Reason indicated as the cause of this return
      tracking_number                          - Tracking number of the return shipment
      carrier                                  - Carrier for the return shipment
      shipping_price                           - Shipping price of the return shipment
      return_line_item.sku_code                - SKU code of the returned item
      return_line_item.unit_count              - Number of units in the line of the return
      return_line_item.serial_number           - Serial number of the device this return is applied to

User Protection Plan Orders.csv:
---------
      order.confirmation_number                - Appropriate Order confirmation number
      create_date                              - Creation date of the protection plan order
      fpp_line_item.serial_number              - Serial number of the device this protection plan is applied to
      fpp_line_item.status                     - Current status of the protection plan for the device