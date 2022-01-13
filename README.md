# Pull Request Labeler

This is a fork of https://github.com/actions/labeler

It introduces `anyor` that can be used to make sure ALL files
match ANY glob from the list.

In the example below, we add the `ci:skip-tests` label
only if all files match one of the glob:

```
'ci:skip-tests':
- anyor:
  - 'README.md'
  - 'docs/*'
  - 'docs/**/*'
  - 'templates/**/*'
  - 'templates/*'
```
