# `noCommaOperator.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/compiler/lint/rules/js/noCommaOperator.test.ts --update-snapshots` to update.

## `no comma operator`

### `0`

```

 unknown:1:1 lint/js/noCommaOperator ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid the comma operator. It can lead to easy mistakes and ambiguous code.

    (0, 1, 2)
     ^^^^^^^

  ℹ If you want multiple expressions, then break it up.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `0: formatted`

```
0, 1, 2;

```

### `1`

```

 unknown:1 lint/js/noCommaOperator ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Avoid the comma operator. It can lead to easy mistakes and ambiguous code.

    test(), rome()
    ^^^^^^^^^^^^^^

  ℹ If you want multiple expressions, then break it up.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `1: formatted`

```
test(), rome();

```

### `2`

```
✔ No known problems!

```

### `2: formatted`

```
foo(0, 1, 2);

```

### `3`

```
✔ No known problems!

```

### `3: formatted`

```
[1, 2];

```

### `4`

```
✔ No known problems!

```

### `4: formatted`

```
[1, undefined, undefined, 3];

```

### `5`

```
✔ No known problems!

```

### `5: formatted`

```
let a;
let b;
let c;

```
