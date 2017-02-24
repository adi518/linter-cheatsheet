# Linters Cheatsheet
It happens to be a major PITA to find these little snippets, so I gather all useful findings here. As a rule of thumb, you should use these as last resort to solve a linting issue.

## JShint
* Suppress a single warning

```
// jshint -<WARNING_IDENTIFIER> // E.g. `W001`
// jshint +<WARNING_IDENTIFIER>

/* Suppress all warnings */

// jshint ignore:start
// jshint ignore:end

// Ignore a line
// jshint ignore:line
```

## SCSS-Lint
* Suppress a single warning

```
// scss-lint:enable <FEATURE_IDENTIFIER> // E.g. `Compass::PropertyWithMixin`
// scss-lint:disable <FEATURE_IDENTIFIER>
```

## Beautify
* Suppress through a section

```
// beautify ignore:start
// beautify ignore:end
```
