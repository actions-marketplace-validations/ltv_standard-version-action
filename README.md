# Standard Version Action

This [Github Action][] calculates the new version based on [Conventional Commits][], updates CHANGELOG, and creates the new git tag. It's powered by [Standard Version][].

## Inputs

This action doesn't accept any inputs. If you want to change a configuration, create a [versionrc file][].

## Example usage

```yaml
- uses: actions/checkout@v2
- name: Configure committer
  run: |
    git config user.name "GitHub Actions Bot"
    git config user.email "<>"
- name: Bump version
  uses: ltv/standard-version@v1
```

[github action]: https://docs.github.com/en/actions
[conventional commits]: https://www.conventionalcommits.org/en/v1.0.0/
[standard version]: https://github.com/conventional-changelog/standard-version
[versionrc file]: https://github.com/conventional-changelog/standard-version#configuration
