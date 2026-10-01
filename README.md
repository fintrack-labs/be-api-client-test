# be-api-client-test

A **[Bruno](https://www.usebruno.com/) API collection** for exercising the FinTrack services locally: register, log in, and call the finance API, without writing a line of code.

Part of [FinTrack Labs](https://github.com/fintrack-labs), a personal learning project on distributed backend design.

## What's inside

- Auth requests: register, login, refresh token, logout, JWKS
- Finance API requests: health, accounts, categories, transactions
- A local environment preconfigured with service URLs

| Variable | Default |
| --- | --- |
| Auth API | `http://127.0.0.1:8081/auth/api` |
| Finance API | `http://localhost:8080/api/v1` |

## Usage

1. Install [Bruno](https://www.usebruno.com/) (or its VS Code extension).
2. Open this folder as a collection.
3. Select the **local** environment.
4. Start the services ([`be-auth-ts`](https://github.com/fintrack-labs/be-auth-ts), [`be-node-ts`](https://github.com/fintrack-labs/be-node-ts)).
5. Run **register**, then **login**, then copy the access token into the environment variable used by the finance requests.

<!-- TODO: jika token otomatis disimpan lewat script Bruno, sesuaikan langkah 5 -->

## Why Bruno instead of Postman?

Collections are plain text files, so they live in Git, show up in diffs and code review, and need no cloud account.

## Notes

- Use dummy credentials only; do not commit real secrets or tokens.

## Related repositories

[`fe-web`](https://github.com/fintrack-labs/fe-web) · [`be-auth-ts`](https://github.com/fintrack-labs/be-auth-ts) · [`be-node-ts`](https://github.com/fintrack-labs/be-node-ts) · [`be-ai-ocr-service`](https://github.com/fintrack-labs/be-ai-ocr-service)
