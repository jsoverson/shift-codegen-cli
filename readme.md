# Shift codegen CLI

Command line tool to generate JavaScript source code from a JSON Shift AST.

## Install

```bash
$ npm install -g shift-codegen-cli
```

## Usage

Usage: shift-codegen ast.json

```bash
# using shift-query to generate a suitable JSON AST
$ shift-query -j example.js Script > ast.json
# regenerating JavaScript source code from that JSON with shift-codegen
$ shift-codegen ast.json
```

If a script is piped to shift-codegen then all arguments are ignored


```bash
$ cat ast.json | shift-codegen
```
