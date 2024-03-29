# GitLab CI validation of publiccode.yml files

[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/italia/publiccode-parser-gitlab-ci/blob/master/LICENSE)

## Usage

This snippet can be included in GitLab CI to validate
[`publiccode.yml`](https://github.com/italia/publiccode.yml)
files using [publiccode-parser-go](https://github.com/italia/publiccode-parser-go).

You can use it in your workflow to check if `publiccode.yml` in your repo is valid.

### Examples

#### Run automatically in the "`test`" stage (simplest configuration)

```yml
# .gitlab-ci.yml

include:
  - https://raw.githubusercontent.com/italia/publiccode-parser-gitlab-ci/main/publiccode-validation.yml
```

#### Run in a custom stage

```yml
# .gitlab-ci.yml

include:
  - https://raw.githubusercontent.com/italia/publiccode-parser-gitlab-ci/main/publiccode-validation.yml

stages:
  - custom_stage

publiccode-parser:
  stage: custom_stage
```
