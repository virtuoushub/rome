# `noDanglingBackslashInRegularExpressions.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/js-compiler/transforms/lint/noDanglingBackslashInRegularExpressions.test.ts --update-snapshots` to update.

## `Dangling backslash in regex`

### `0`

```javascript
Object {
  src: 'let foo = /\\/;foo;'
  suppressions: Array []
  diagnostics: Array [
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/noDanglingBackslash'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Dangling backslash in a regular expression'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 12
          index: 13
          line: 1
        }
        start: Object {
          column: 11
          index: 11
          line: 1
        }
      }
    }
  ]
}
```

### `1`

```javascript
Object {
  src: 'let foo = /\\\\\\/;foo;'
  suppressions: Array []
  diagnostics: Array [
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/noDanglingBackslash'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Dangling backslash in a regular expression'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 14
          index: 15
          line: 1
        }
        start: Object {
          column: 13
          index: 13
          line: 1
        }
      }
    }
  ]
}
```

### `2`

```javascript
Object {
  src: 'let foo = /\\/\\/;\\/;foo;'
  suppressions: Array []
  diagnostics: Array [
    Object {
      origins: Array [Object {category: 'js-parser'}]
      description: Object {
        category: 'parse/js'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Expecting Unicode escape sequence \\uXXXX'}
      }
      location: Object {
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 17
          index: 17
          line: 1
        }
        start: Object {
          column: 17
          index: 17
          line: 1
        }
      }
    }
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/noDanglingBackslash'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Dangling backslash in a regular expression'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 14
          index: 15
          line: 1
        }
        start: Object {
          column: 13
          index: 13
          line: 1
        }
      }
    }
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/undeclaredVariables'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Undeclared variable <emphasis>\0</emphasis>'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 18
          index: 18
          line: 1
        }
        start: Object {
          column: 16
          index: 16
          line: 1
        }
      }
    }
  ]
}
```

### `3`

```javascript
Object {
  src: 'let foo = /\\/\\/;\\/\n    foo;'
  suppressions: Array []
  diagnostics: Array [
    Object {
      origins: Array [Object {category: 'js-parser'}]
      description: Object {
        category: 'parse/js'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Expecting Unicode escape sequence \\uXXXX'}
      }
      location: Object {
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 17
          index: 17
          line: 1
        }
        start: Object {
          column: 17
          index: 17
          line: 1
        }
      }
    }
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/noDanglingBackslash'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Dangling backslash in a regular expression'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 14
          index: 15
          line: 1
        }
        start: Object {
          column: 13
          index: 13
          line: 1
        }
      }
    }
    Object {
      origins: Array [Object {category: 'lint'}]
      description: Object {
        category: 'lint/undeclaredVariables'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Undeclared variable <emphasis>\0</emphasis>'}
      }
      location: Object {
        filename: 'unknown'
        language: 'js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 18
          index: 18
          line: 1
        }
        start: Object {
          column: 16
          index: 16
          line: 1
        }
      }
    }
  ]
}
```