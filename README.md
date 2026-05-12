# cloud-nx-demo

[![Capawesome](https://github.com/capawesome-team/cloud-nx-demo/actions/workflows/capawesome.yml/badge.svg)](https://github.com/capawesome-team/cloud-nx-demo/actions/workflows/capawesome.yml)

A demo project that shows how to build a [Capacitor](https://capacitorjs.com/) app in an [Nx](https://nx.dev/) monorepo using [Capawesome Cloud](https://capawesome.io/cloud/).

## Stack

- [Nx](https://nx.dev/) monorepo
- [Capacitor](https://capacitorjs.com/) — Android + iOS
- [Ionic](https://ionicframework.com/) + [Angular](https://angular.dev/)
- [npm](https://www.npmjs.com/) — package manager

## Continuous Integration

[`.github/workflows/capawesome.yml`](.github/workflows/capawesome.yml) builds the app on every push to `main`, on pull requests, and on manual dispatch using the [Capawesome CLI](https://capawesome.io/docs/cloud/cli/).

A [`capawesome.config.json`](capawesome.config.json) file at the repository root tells Capawesome Cloud where the Capacitor app lives within the monorepo and how to install dependencies and build the web assets.

### Required GitHub Secrets

| Secret | Description |
| --- | --- |
| `CAPAWESOME_CLOUD_TOKEN` | API token for Capawesome Cloud. |
| `CAPAWESOME_CLOUD_APP_ID` | ID of the corresponding app in Capawesome Cloud. |

## License

See [LICENSE](LICENSE).
