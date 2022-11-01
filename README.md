<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Standard Deviation

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> [Degenerate][degenerate-distribution] distribution [standard deviation][standard-deviation].

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

The [variance][standard-deviation] for a [degenerate][degenerate-distribution] random variable is

<!-- <equation class="equation" label="eq:degenerate_stdev" align="center" raw="\operatorname{SD}\left( X \right) = 0" alt="Standard deviation for a degenerate distribution."> -->

<div class="equation" align="center" data-raw-text="\operatorname{SD}\left( X \right) = 0" data-equation="eq:degenerate_stdev">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@e1fbdee688c5409e4cc6b0cd06d90b1cd2abd67c/lib/node_modules/@stdlib/stats/base/dists/degenerate/stdev/docs/img/equation_degenerate_stdev.svg" alt="Standard deviation for a degenerate distribution.">
    <br>
</div>

<!-- </equation> -->

where `μ` is the constant value of the distribution.

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

```javascript
import stdev from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-degenerate-stdev@esm/index.mjs';
```

#### stdev( mu )

Returns the [standard deviation][standard-deviation] of a [degenerate][degenerate-distribution] distribution with constant value `mu`.

```javascript
var v = stdev( 10.0 );
// returns 0.0

v = stdev( -0.5 );
// returns 0.0

v = stdev( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@esm/index.mjs';
import stdev from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-degenerate-stdev@esm/index.mjs';

var mu;
var v;
var i;

for ( i = 0; i < 10; i++ ) {
    mu = randu();
    v = stdev( mu );
    console.log( 'µ: %d, SD(X;µ): %d', mu.toFixed( 4 ), v.toFixed( 4 ) );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/stats-base-dists-degenerate-stdev.svg
[npm-url]: https://npmjs.org/package/@stdlib/stats-base-dists-degenerate-stdev

[test-image]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/stats-base-dists-degenerate-stdev/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/stats-base-dists-degenerate-stdev?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/stats-base-dists-degenerate-stdev.svg
[dependencies-url]: https://david-dm.org/stdlib-js/stats-base-dists-degenerate-stdev/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/tree/deno
[umd-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/tree/umd
[esm-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/tree/esm
[branches-url]: https://github.com/stdlib-js/stats-base-dists-degenerate-stdev/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/stats-base-dists-degenerate-stdev/main/LICENSE

[degenerate-distribution]: https://en.wikipedia.org/wiki/Degenerate_distribution

[standard-deviation]: https://en.wikipedia.org/wiki/Standard_deviation

</section>

<!-- /.links -->
