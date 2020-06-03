# assert-sass
Assertion function library for Dart Sass

## Installation

```
$ npm install @gyugyu/assert-sass sass
```

## Example

```scss
@use '@gyugyu/assert-sass' as assert;

@function sum($a, $b) {
  @return $a + $b;
}

$result: assert.equals(sum(2, 3), 5);
```

## API

* `assert.equals($expected, $actual)`
* `assert.not-null($value)`
* `assert.contains-all-keys($map, $keys)`
