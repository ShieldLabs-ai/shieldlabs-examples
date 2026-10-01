# signup-gating example

Allow, verify or hold a new account based on the ShieldLabs verdict for the signup request and on how many accounts the same device ID has already created.

The runnable app is being prepared. The flow it will show: the browser sends the `requestId` of a fresh identification with the action, the server reads the verdict for it from the History API and applies the policy described above.
