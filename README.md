# hledger-vscode README

Language support for [HLedger](http://hledger.org/) command-line accounting [journal files](http://hledger.org/journal.html).

## Features

- Syntax highlighting

![Syntax Highlighting](images/screenshot.png)

![Highlighting of tags](images/feature-tags.png)

### Todo:

- Account Tab Completion

## Known Issues

- No highlighting of amounts (numbers)

## Updating Tests

We have golden file tests under `tests/cases`, containing example
`.in.hledger` files, and syntax-highlighted `.want` files. Run the tests with
`npm test`.

If you've examined the differences and they're expected, rebuild the golden files by running
`ts-node tests/main.ts tests/cases/*.in.hledger`.
