# Personal balance widget

This is a personal-use project to show an account balance and a credit-card amount owed together in a phone widget. The planned flow is: an account owner connects their own accounts through Plaid Link; a Cloudflare Worker requests balance data through Plaid; the widget displays the balances and their difference.

## Scope

- One user, using only accounts they authorize.
- Read-only balance display. No payments, transfers, trading, or other money movement.
- Plaid handles account linking. The app is designed to use Plaid access tokens rather than bank passwords.
- The project is in setup and review. It is not represented here as a deployed service or an approved Plaid production integration.

## Data handling plan

Plaid and Cloudflare would process the data needed to retrieve and display balances. The planned app would keep its Plaid credentials and access tokens out of this public repository, restrict access to the balance endpoint, and avoid selling or publishing account data. Actual production data handling will depend on the final deployed implementation and service configuration.

This repository currently provides a public description for project verification. Application code will be added after its authentication and data-handling review.
