# prbuild-orb

[![CircleCI](https://circleci.com/gh/netgaintechnology/orb-prebuild-orb.svg?style=svg)](https://circleci.com/gh/netgaintechnology/orb-prebuild-orb) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)

An orb managing pre-build phase jobs such as linting and formating.

## Usage

For full usage guidelines, see the [orb registry listing](http://circleci.com/orbs/registry/orb/netgaintechnology/orb-prebuild-orb).

### Example

Following is an example of a linting pipeline and making use of multiple jobs from this orb.

```yaml
version: 2.1

  orbs:
    linting-tools: netgaintechnology/prebuild-orb@x.y.z

  workflows:
    version: 2
    linting:
      jobs:
        - linting-tools/yaml_lint
        - linting-tools/markdown_lint
        - liting-tools/json_lint
```

## Contributing

We welcome [issues](https://github.com/netgaintechnology/orb-prebuild-orb/issues) to and [pull requests](https://github.com/netgaintechnology/orb-prebuild-orb/pulls) against this repository!
