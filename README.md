# ShieldLabs examples

Example apps that read a ShieldLabs verdict on the server and act on it: signup gating, checkout risk, metered content and account sharing.

> The scenario apps are being prepared. Until they land here, start from the SDK quick starts in the [ShieldLabs documentation](https://docs.shieldlabs.ai).

## How every example works

1. The browser runs an identification with `@shieldlabs-ai/js` (or a framework package) and sends the `requestId` along with the form or request.
2. The server reads the verdict for that request ID from the History API with a server SDK, or receives it by a signed webhook.
3. The server acts on the Risk Score, the three risk bands (trusted 0-29, suspicious 30-59, dangerous 60-100), the detection flags and the identifiers, for example how many accounts one device ID has already created.

## Scenarios

| Folder | What it shows |
|---|---|
| [`signup-gating/`](./signup-gating) | Allow, verify or hold a new account based on the verdict and on how many accounts the device already has |
| [`checkout-risk/`](./checkout-risk) | Route risky orders to review before payment |
| [`paywall/`](./paywall) | Keep metered or gated content limits per device, not per cookie |
| [`account-sharing/`](./account-sharing) | Spot one paid account used from many devices |

## About ShieldLabs

ShieldLabs identifies visitors and scores risk with 300+ device, network and behavior signals, so you can detect risky users and stop abuse of your product.

- Website: [shieldlabs.ai](https://shieldlabs.ai)
- Documentation: [docs.shieldlabs.ai](https://docs.shieldlabs.ai)
- Start free: [app.shieldlabs.ai](https://app.shieldlabs.ai)

## License

[MIT](./LICENSE)
