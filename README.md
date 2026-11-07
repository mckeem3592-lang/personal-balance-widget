# Personal balance widget

This is a single-user project to show an account balance and a credit-card amount owed together in an iPhone widget. The owner connects their own accounts through Plaid Link. A Cloudflare Worker retrieves balance data, and the widget displays the balances and their difference.

## Scope and status

- Read-only balance display; no payments, transfers, trading, or other money movement.
- The Worker is deployed, two accounts have been linked, and the balance endpoint returns the selected values with a verified difference.
- The iPhone widget script is configured; its on-device display still needs confirmation.
- This is a personal trial project, not a company or a claim of approved long-term production access.

## Data handling

Plaid processes account linking and balance requests. Cloudflare hosts the Worker and stores Plaid access tokens in a private KV namespace. Plaid credentials, selected account IDs, and the widget access key are Worker secrets; no bank passwords or account balances are published here. The balance endpoint requires an access key. Data is for the owner's own display and is not intended for sale or public sharing.

This public repository provides a project description for verification. Application source is kept in a separate private repository.
