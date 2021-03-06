<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Contributing guidelines](#contributing-guidelines)
  - [Sign the CLA](#sign-the-cla)
  - [Contributing A Patch](#contributing-a-patch)
  - [Pre-check before submitting a PR](#pre-check-before-submitting-a-pr)
  - [Build and push images](#build-and-push-images)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Contributing guidelines

## Sign the CLA

Kubernetes projects require that you sign a Contributor License Agreement (CLA) before we can accept your pull requests.  Please see https://git.k8s.io/community/CLA.md for more info

## Contributing A Patch

1. Submit an issue describing your proposed change to the repo in question.
1. The [repo owners](OWNERS) will respond to your issue promptly.
1. If your proposed change is accepted, and you haven't already done so, sign a Contributor License Agreement (see details above).
1. Fork the desired repo, develop and test your code changes.
1. Submit a pull request.

## Pre-check before submitting a PR

After your PR is ready to commit, please run following commands to check your code:

```shell
make check
make test
```

## Build and push images
Make sure your code build passed:

```shell
export REGISTRY=<your-docker-registry>
make build-push-images
```

Now, you can follow the [getting started guide](./README.md#getting-started) to work with the Cluster API Provider IBM Cloud.
