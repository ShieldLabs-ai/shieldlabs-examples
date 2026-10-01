# checkout-risk example

Route risky orders to manual review before payment, based on the verdict for the checkout request and on the detection flags.

The runnable app is being prepared. The flow it will show: the browser sends the `requestId` of a fresh identification with the action, the server reads the verdict for it from the History API and applies the policy described above.
