# deno_is_absolute [deprecated]

[![tag](https://img.shields.io/github/release/justjavac/deno_is_absolute)](https://github.com/justjavac/deno_is_absolute/releases)
[![Build Status](https://github.com/justjavac/deno_is_absolute/workflows/ci/badge.svg?branch=master)](https://github.com/justjavac/deno_is_absolute/actions)
[![license](https://img.shields.io/github/license/justjavac/deno_is_absolute)](https://github.com/justjavac/deno_is_absolute/blob/master/LICENSE)

Whether the filepath is a **absolute** file path.

⚠️ **Please Use Deno Standard Library.**

```ts
import { isAbsolute } from "https://deno.land/std/path/mod.ts";
```

## Usage

```ts
import isAbsolute from "https://deno.land/x/is_absolute/mod.ts";

// return true
isAbsolute('/home/foo')
isAbsolute('/home/foo/..')
isAbsolute('/')
isAbsolute('//')
isAbsolute('//foo')
isAbsolute('c:\\')
isAbsolute('c:/')
isAbsolute('c://')
isAbsolute('C:/Users/')
isAbsolute('C:\\Users\\')

// return false
isAbsolute("bar/")
isAbsolute("./baz")
isAbsolute("c")
isAbsolute("c;")
isAbsolute("C:cwd/another")
isAbsolute("C:cwd\\another")
isAbsolute("foo/bar")
isAbsolute("foo\\bar")
```

## License

[deno_is_absolute](https://github.com/justjavac/deno_is_absolute) is released under the MIT License. See the bundled [LICENSE](./LICENSE) file for details.
