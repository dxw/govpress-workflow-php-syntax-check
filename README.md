# GovPress Workflow: PHP Check Syntax

This repo holds a reusable workflow for checking PHP files in GovPress projects.

## Usage

In calling .yml workflow file:
```
name: PHP syntax check

on: [push, pull_request]

jobs:

  php-syntax-check:
    uses: dxw/govpress-workflow-php-syntax-check/.github/workflows/php-syntax-check.yml@v1
```

## Test
Can be tested locally using act, for example in calling repo:
```
act -W '.github/workflows/php-syntax-check.yml';
```

To test errors locally, will need a PHP error added to a file on default (main) branch.
