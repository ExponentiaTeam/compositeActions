# compositeActions
Composite actions for CI

Example:

rubocop:
    name: rubocop
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - uses: exponentiaTeam/compositeActions/yarnInstall
    - run: bundle exec rubocop
