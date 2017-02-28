# Linter Cheatsheet

It happens to be a major PITA to find these little snippets, so I gather all useful findings here. As a rule of thumb, you should use these as last resort to solve a linting issue.

** Some `JSlint` suppressors work with `JSHint`, YMMV. For `JShint/JSLint` compatibility, `space` after a comment identifier (`/*`) must be omitted.

## ESLint

<http://eslint.org/docs/rules/>

- Suppress all warnings

```
/* eslint-disable */
```
- Suppress all warnings for a single line

```
// eslint-disable-line
```

## JShint

- Suppress environment warnings

```
// jslint browser: true
// jslint jquery: true
// jshint esversion: 6
```

- Suppress undefined global variables. **

```
/*global <var1>, <var2>, ... */
```

- Suppress exported/unused global variables. **

```
/*exported <var1>, <var2>, ... */
```

- Suppress a single warning. Example: `// jshint -W001`

```
// jshint -<*>
// jshint +<*>
```

- Suppress all warnings

```
// jshint ignore:start
// jshint ignore:end
```

- Suppress all warnings for a single line

```
// jshint ignore:line
```

## SCSS-Lint

- Suppress a single warning. Example: `// scss-lint:enable Compass::PropertyWithMixin`

```
// scss-lint:enable <*>
// scss-lint:disable <*>
```

## Pug-lint (was Jade)

<https://github.com/pugjs/pug-lint/blob/master/docs/rules.md>

## Beautify

- Suppress through a section (must be a block-comment)

```
/* beautify ignore:start */
/* beautify ignore:end */
```
