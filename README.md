# GitLab CI validation of publiccode.yml files

[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/italia/publiccode-parser-gitlab-ci/blob/master/LICENSE)

## Usage

This snippet can be included in GitLab CI to validate
[`publiccode.yml`](https://github.com/italia/publiccode.yml)
files using [publiccode-parser-go](https://github.com/italia/publiccode-parser-go).

You can use it in your workflow to check if `publiccode.yml` in your repo is valid.

### Example

```yml
# .gitlab-ci.yml
include:
  - https://raw.githubusercontent.com/italia/publiccode-parser-gitlab-ci/main/publiccode-validation.yml
```
