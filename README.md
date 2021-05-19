# Setup AWS Copilot

> 👩‍✈️A GitHub Action for setting up the [AWS Copilot command line interface](https://github.com/aws/copilot-cli)

## fork info

This is Tipsre for of `softprops/setup-aws-copilot`. Intial reason was to have udpated dependencies. Outdated one caused the action to fail. Second reason, that popped up later on is to switch to Tipser fork of `copilot-cli` -> https://github.com/Tipser/copilot-cli.

## usage

Add a step to your workflow to install AWS Copilot

```yml
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Setup AWS Copilot
      uses: Tisper/setup-aws-copilot@v3
```

#### inputs

| Name        | Type    | Description                                                     |
|-------------|---------|-----------------------------------------------------------------|
| `version`      | string  | version of [Copilot cli release](https://github.com/aws/copilot-cli/releases) defaults to latest version                |


Doug Tangren (softprops) 2020.
