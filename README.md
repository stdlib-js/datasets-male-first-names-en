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

# Male First Names

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> A [list][@ward:2002a] of common male first names in English speaking countries.

<section class="installation">

## Installation

```bash
npm install @stdlib/datasets-male-first-names-en
```

</section>

<section class="usage">

## Usage

```javascript
var names = require( '@stdlib/datasets-male-first-names-en' );
```

#### names()

Returns a [list][@ward:2002a] of common male first names (also known as [given][given-name] or personal names) in English speaking countries.

```javascript
var data = names();
/* returns
    [
        'Aaron',
        'Ab',
        'Abba',
        'Abbe',
        'Abbey',
        'Abbie',
        'Abbot',
        'Abbott',
        ...
    ]
*/
```

</section>

<!-- /.usage -->

<section class="examples">

<!-- TODO: more creative example. -->

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var floor = require( '@stdlib/math-base-special-floor' );
var randu = require( '@stdlib/random-base-randu' );
var names = require( '@stdlib/datasets-male-first-names-en' );

var data = names();
var len = data.length;
var idx;
var i;

// Select random names from the list...
for ( i = 0; i < 100; i++ ) {
    idx = floor( randu()*len );
    console.log( data[ idx ] );
}
```

</section>

<!-- /.examples -->

* * *

<section class="cli">

## CLI

<section class="installation">

## Installation

To use the module as a general utility, install the module globally

```bash
npm install -g @stdlib/datasets-male-first-names-en
```

</section>

<section class="usage">

### Usage

```text
Usage: male-first-names-en [options]

Options:

  -h,    --help                Print this message.
  -V,    --version             Print the package version.
```

</section>

<!-- /.usage -->

<section class="examples">

### Examples

```bash
$ male-first-names-en
Aaron
Ab
Abba
Abbe
...
```

</section>

<!-- /.examples -->

</section>

<!-- /.cli -->

* * *

<section class="references">

## References

-   Ward, Grady. 2002. "Moby Word II." <http://www.gutenberg.org/files/3201/3201.txt>.

</section>

<!-- /.references -->

<!-- <license> -->

## License

The data files (databases) are licensed under an [Open Data Commons Public Domain Dedication & License 1.0][pddl-1.0] and their contents are licensed under [Creative Commons Zero v1.0 Universal][cc0]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-male-first-names-en.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-male-first-names-en

[test-image]: https://github.com/stdlib-js/datasets-male-first-names-en/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/datasets-male-first-names-en/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-male-first-names-en/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-male-first-names-en?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-male-first-names-en
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-male-first-names-en/main

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/datasets-male-first-names-en/main/LICENSE

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

[given-name]: https://en.wikipedia.org/wiki/Given_name

[@ward:2002a]: http://www.gutenberg.org/files/3201/3201.txt

</section>

<!-- /.links -->
