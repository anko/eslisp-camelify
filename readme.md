# eslisp-camelify [![](https://img.shields.io/npm/v/eslisp-camelify.svg?style=flat-square)][1] [![](https://img.shields.io/travis/anko/eslisp-camelify.svg?style=flat-square)][2] [![](https://img.shields.io/badge/eslisp_chat-gitter_%E2%86%92-blue.svg?style=flat-square)][3]

An [eslisp][4] macro that rewrites all atoms in its arguments from
`dash-separated` to `camelCase`, but otherwise touches nothing.

Handy if you prefer lisp-like `dash-separated-variables`.

## Example

    (macro camelify (require "eslisp-camelify"))
    (camelify
      (explain-that (the-answer-is 42)))

↓

    explainThat(theAnswerIs(42));

It probably makes good sense to use this as a [transform macro][5] to wrap your
whole program though:

    eslc -t eslisp-camelify < input.esl > output.js

See [the tests][6] for fuller usage.

## License

[ISC][7].

[1]: https://www.npmjs.com/package/eslisp-camelify
[2]: https://travis-ci.org/anko/eslisp-camelify
[3]: https://gitter.im/anko/eslisp
[4]: https://github.com/anko/eslisp
[5]: https://github.com/anko/eslisp/blob/master/doc/how-macros-work.markdown#transform-macros
[6]: test.esl
[7]: http://opensource.org/licenses/ISC
