# compositeActions
Composite actions for CI

## Current actions:
- Cache for Yarn Install
- Cache for Bundle Install

## Example:
```
  rubocop:
    name: rubocop
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - uses: ExponentiaTeam/compositeActions/bundleInstall@master
    - run: bundle exec rubocop
```