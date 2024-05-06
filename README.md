<<<<<<< HEAD
# docker-typescript-action-template
[![Build Image](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/build-image.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/build-image.yml)
[![Docker Tag](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/docker-tag.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/docker-tag.yml)
[![Git Tag Semver From Label](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/git-tag-semver-from-label.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/git-tag-semver-from-label.yml)
[![Trigger Update From Template](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/trigger-update-from-template.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-typescript-action-template/actions/workflows/trigger-update-from-template.yml)
[![codecov](https://codecov.io/gh/infrastructure-blocks/docker-typescript-action-template/graph/badge.svg?token=S1OANU9UMZ)](https://codecov.io/gh/infrastructure-blocks/docker-typescript-action-template)
=======
# docker-action-template
[![Build](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/build.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/build.yml)
[![Release](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/release.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/release.yml)
[![Git Tag](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/git-tag.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/git-tag.yml)
[![Trigger Update From Template](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/trigger-update-from-template.yml/badge.svg)](https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/trigger-update-from-template.yml)
>>>>>>> template/master

[//]: # ([![Update From Template]&#40;https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/update-from-template.yml/badge.svg&#41;]&#40;https://github.com/infrastructure-blocks/docker-action-template/actions/workflows/update-from-template.yml&#41;)

A template repository for GitHub Actions hosted as docker images on registries.

## Instantiation checklist

- Do a global search & replace for `docker-action-template` and replace it with the name of your repository
- Remove the [trigger update from template workflow](.github/workflows/trigger-update-from-template.yml)
<<<<<<< HEAD
- Rename the docker image/container in [docker compose file](./docker/docker-compose.yml)
- Edit the package.json to reflect the action's name and links
- Run `nvm install`
- Run `npm install`
- Replace the self-test section of the [build-image workflow](.github/workflows/build-image.yml).
- Set up code coverage
- Update the status badges:
    - Remove the `Trigger Update From Template` status badge.
    - Add the `Update From Template` status badge.
    - Rename the rest of the links to point to the right repository.
- Replace the summary and the action usage section in this document.
=======
- Remove the `Trigger Update From Template` status badge
- Uncomment the `Update From Template` status badge.
- Replace the self-test section of the [build-image workflow](.github/workflows/build.yml)
- Replace the summary and the action usage section in this readme.
- Prepare the [changelog](CHANGELOG.md) for the first version of the module that will be released.
>>>>>>> template/master

## Inputs

|     Name      | Required | Description      |
|:-------------:|:--------:|------------------|
| example-input |   true   | A useless input. |

## Outputs

|      Name      | Description                    |
|:--------------:|--------------------------------|
| example-output | An equivalently useless output |

## Permissions

|     Scope     | Level | Reason   |
|:-------------:|:-----:|----------|
| pull-requests | read  | Because. |

## Usage

```yaml
- uses: docker://public.ecr.aws/infrastructure-blocks/docker-typescript-action-template:v1
  with:
    example-input: hello
```
