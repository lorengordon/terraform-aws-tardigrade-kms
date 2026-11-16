## terraform-aws-tardigrade-kms Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).

### 2.0.0

**Released**: 2021.01.20

**Commit Delta**: [Change from 1.0.0 release](https://github.com/plus3it/terraform-aws-tardigrade-kms/compare/1.0.0...2.0.0)

**Summary**:

*   Remove the `create_keys` variable. The `keys` variable is now required.
    Callers that set `create_keys` must remove it.

### 1.0.0

**Released**: 2021.01.08

**Commit Delta**: [Change from 0.0.2 release](https://github.com/plus3it/terraform-aws-tardigrade-kms/compare/0.0.2...1.0.0)

**Summary**:

*   Always create the keys in `keys`. The `create_keys` variable no longer has
    an effect.
*   Set the type of `keys` to `list(any)`
*   Remove the Terratest Go module and the `no_create_key` test

### 0.0.2

**Released**: 2020.01.02

**Commit Delta**: [Change from 0.0.1 release](https://github.com/plus3it/terraform-aws-tardigrade-kms/compare/0.0.1...0.0.2)

**Summary**:

*   Expose key rotation variable

### 0.0.1

**Released**: 2019.12.31

**Commit Delta**: [Change from 0.0.0 release](https://github.com/plus3it/terraform-aws-tardigrade-kms/compare/0.0.0...0.0.1)

**Summary**:

*   Simplifying module

### 0.0.0

**Commit Delta**: N/A

**Released**: 2019.12.12

**Summary**:

*   Initial release!
