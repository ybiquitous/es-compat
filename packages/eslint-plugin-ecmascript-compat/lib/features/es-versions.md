# ECMAScript features by version

Static detectability of recently-added features

- ❌ = not statically detectable
- 😐 = statically detectable, but chance of false positives
- 👎 = statically detectable, but not worth the false positives

### ES2021

| Name                                 | ESLint / eslint-plugin-es-x          | Chrome since |
| ------------------------------------ | ------------------------------------ | ------------ |
| Logical Assignment \|\|=, \&\&=, ??= | es-x/no-logical-assignment-operators | 85           |
| Numeric separators                   | es-x/no-numeric-separators           | 75           |
| `Promise.any`                        | es-x/no-promise-any                  | 85           |
| `String.prototype.replaceAll`        | 😐 no-restricted-properties          | 85           |
| `WeakRef and FinalizationRegistry`   | es-x/no-weakrefs                     | 84           |

### ES2020

| Name                        | ESLint / eslint-plugin-es-x          | Chrome since |
| --------------------------- | ------------------------------------ | ------------ |
| `Atomics.{notify, wait}`    | no-restricted-properties             | 68           |
| `BigInt`                    | es-x/no-bigint                       | 67           |
| Dynamic `import()`          | es-x/no-dynamic-import               | 63           |
| `globalThis`                | es-x/no-global-this                  | 71           |
| `import.meta`               | es-x/no-import-meta                  | 64           |
| Module namespace exports    | es-x/no-export-ns-from               | 72           |
| Nullish coalescing (`??`)   | es-x/no-nullish-coalescing-operators | 80           |
| Optional chaining (`?.`)    | es-x/no-optional-chaining            | 80           |
| `Promise.allSettled`        | es-x/no-promise-all-settled          | 76           |
| `String.prototype.matchAll` | 😐 no-restricted-syntax              | 73           |

### ES2019

| Name                                  | ESLint / eslint-plugin-es-x    | Chrome since |
| ------------------------------------- | ------------------------------ | ------------ |
| `Array.prototype.{flat, flatMap}`     | 😐 no-restricted-syntax        | 69           |
| JSON superset                         | es-x/no-json-superset          | 66           |
| `Object.fromEntries`                  | es-x/no-object-fromentries     | 73           |
| Optional `catch` binding              | es-x/no-optional-catch-binding | 66           |
| Revised `Function.prototype.toString` | ❌                             |
| Stable `Array.prototype.sort`         | ❌                             |
| `String.prototype.trimX` methods      | 😐 no-restricted-syntax        | 66           |
| `Symbol.prototype.description`        | 👎 no-restricted-syntax        | 70           |
| Well-formed `JSON.stringify`          | ❌                             |

### ES2018

| Name                                | ESLint / eslint-plugin-es-x             | Chrome since |
| ----------------------------------- | --------------------------------------- | ------------ |
| Async iteration (loop & generators) | es-x/no-async-iteration                 | 63           |
| Object rest and spread operators    | es-x/no-rest-spread-properties          | 60           |
| `Promise.prototype.finally`         | 😐 no-restricted-syntax                 | 63           |
| RegExp look-behind assertions       | es-x/no-regexp-lookbehind-assertions    | 62           |
| RegExp named capture groups         | es-x/no-regexp-named-capture-groups     | 64           |
| RegExp `/s` (dotAll) flag           | es-x/no-regexp-s-flag                   | 62           |
| RegExp Unicode property escapes     | es-x/no-regexp-unicode-property-escapes | 64           |

### ES2017

| Name                                  | ESLint / eslint-plugin-es-x              | Chrome since |
| ------------------------------------- | ---------------------------------------- | ------------ |
| Async functions                       | es-x/no-async-functions                  | 55           |
| Atomics                               | es-x/no-atomics                          | 68           |
| `Object.entries`                      | es-x/no-object-entries                   | 54           |
| `Object.getOwnPropertyDescriptors`    | es-x/no-object-getownpropertydescriptors | 54           |
| `Object.values`                       | es-x/no-object-values                    | 54           |
| SharedArrayBuffer                     | es-x/no-shared-array-buffer              | 68           |
| `String.prototype.{padStart, padEnd}` | 😐 no-restricted-syntax                  | 57           |
| Trailing commas in parameter lists    | es-x/no-trailing-function-commas         | 58           |

### ES2016

| Name                       | ESLint / eslint-plugin-es-x   | Chrome since |
| -------------------------- | ----------------------------- | ------------ |
| `Array.prototype.includes` | 😐 no-restricted-syntax       | 47           |
| Exponentiation operator    | es-x/no-exponential-operators | 52           |
