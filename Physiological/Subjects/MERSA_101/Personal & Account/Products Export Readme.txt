Products Data Export

This portion of your data export includes data on your Premium subscriptions

User Premium Subscriptions.csv:
---------
      provider_id            - subscription provider, apple or google
      sku                    - Fitbit name of premium product
      product_description    - premium product short description
      product_reccurence     - premium product recurrence
      start_date             - the date premium subscription started
      valid_until            - the date premium subscription is valid until
      user_cancellation_date - the date premium subscription was cancelled by the user
      trial_period           - 'TRUE' means that subscription in the free trial status
      receipt                - encoded Apple or Google receipt with your subscriptions data
      fatal_renewal_error    - if 'TRUE' subscription renewal will not be retried
      grant_bundle           - the name of features set included into the subscription

User Premium Transactions.csv:
---------
      provider_id             - subscription provider, apple or google
      sku                     - Fitbit name of premium product
      timestamp               - date and time of the transaction
      provider_transaction_id - transaction identifier received from Apple or Google