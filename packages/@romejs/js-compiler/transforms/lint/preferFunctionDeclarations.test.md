# `preferFunctionDeclarations.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/js-compiler/transforms/lint/preferFunctionDeclarations.test.ts --update-snapshots` to update.

## `prefer function declarations`

### `0`

```javascript
Object {
  src: 'function foo() {}\n'
  suppressions: Array []
  diagnostics: Array [
    Object {
      category: 'lint/preferFunctionDeclarations'
      filename: 'unknown'
      fixable: true
      language: 'js'
      message: 'Use a function declaration instead of a const function'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 26
        index: 26
        line: 1
      }
      start: Object {
        column: 12
        index: 12
        line: 1
      }
    }
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused variable <emphasis>foo</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 9
        index: 9
        line: 1
      }
      start: Object {
        column: 6
        index: 6
        line: 1
      }
    }
  ]
}
```

### `1`

```javascript
Object {
  src: 'function foo() {}\n'
  suppressions: Array []
  diagnostics: Array [
    Object {
      category: 'lint/preferFunctionDeclarations'
      filename: 'unknown'
      fixable: true
      language: 'js'
      message: 'Use a function declaration instead of a const function'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 20
        index: 20
        line: 1
      }
      start: Object {
        column: 12
        index: 12
        line: 1
      }
    }
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused variable <emphasis>foo</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 9
        index: 9
        line: 1
      }
      start: Object {
        column: 6
        index: 6
        line: 1
      }
    }
  ]
}
```

### `2`

```javascript
Object {
  src: 'const foo = () => {\n  this;\n};\n'
  suppressions: Array []
  diagnostics: Array [
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused variable <emphasis>foo</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 9
        index: 9
        line: 1
      }
      start: Object {
        column: 6
        index: 6
        line: 1
      }
    }
  ]
}
```

### `3`

```javascript
Object {
  src: 'function foo() {\n  function bar() {\n    this;\n  }\n}\n'
  suppressions: Array []
  diagnostics: Array [
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused function <emphasis>bar</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 31
        index: 31
        line: 1
      }
      start: Object {
        column: 28
        index: 28
        line: 1
      }
    }
    Object {
      category: 'lint/preferFunctionDeclarations'
      filename: 'unknown'
      fixable: true
      language: 'js'
      message: 'Use a function declaration instead of a const function'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 42
        index: 42
        line: 1
      }
      start: Object {
        column: 12
        index: 12
        line: 1
      }
    }
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused variable <emphasis>foo</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 9
        index: 9
        line: 1
      }
      start: Object {
        column: 6
        index: 6
        line: 1
      }
    }
  ]
}
```

### `4`

```javascript
Object {
  src: 'const foo: string = function() {};\n'
  suppressions: Array []
  diagnostics: Array [
    Object {
      category: 'lint/unusedVariables'
      filename: 'unknown'
      language: 'js'
      message: 'Unused variable <emphasis>foo</emphasis>'
      mtime: undefined
      sourceType: 'module'
      origins: Array [Object {category: 'lint'}]
      end: Object {
        column: 17
        index: 17
        line: 1
      }
      start: Object {
        column: 6
        index: 6
        line: 1
      }
    }
  ]
}
```
