# Linter Cheatsheet
It happens to be a major PITA to find these little snippets, so I gather all useful findings here. As a rule of thumb, you should use these as last resort to solve a linting issue.

Some `JSlint` suppressors work with `JSHint`, YMMV.

## JShint
* Suppress environment warnings

```
// jslint browser: true
// jslint jquery: true
// jshint esversion: 6
```
* Suppress a single warning. Example: `// jshint -W001`

```
// jshint -<*>
// jshint +<*>
```
* Suppress all warnings

```
// jshint ignore:start
// jshint ignore:end
```
* Suppress all warnings on a single line

```
// jshint ignore:line
```

## SCSS-Lint
* Suppress a single warning. Example: `// scss-lint:enable Compass::PropertyWithMixin`

```
// scss-lint:enable <*>
// scss-lint:disable <*>
```

## Beautify
* Suppress through a section

```
// beautify ignore:start
// beautify ignore:end
```
