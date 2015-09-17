# eslisp-camelify [![](https://img.shields.io/npm/v/eslisp-camelify.svg?style=flat-square)][1] [![](https://img.shields.io/travis/anko/eslisp-camelify.svg?style=flat-square)][2] [![](https://img.shields.io/badge/eslisp_chat-gitter_%E2%86%92-blue.svg?style=flat-square)][3]

An [eslisp][4] macro that rewrites all atoms in its arguments from
`dash-separated` to `camelCase`, but otherwise touches nothing.

Handy if you prefer lisp-like `dash-separated-variables`.

## Example

    (macro camelify (require "/path/to/eslisp-camelify/index.js"))
    (camelify (explain-that (the-answer-is 42)))

↓

    explainThat(theAnswerIs(42));

See [the tests][5] for fuller usage.

## License

[ISC][6].

[1]: https://www.npmjs.com/package/eslisp-camelify
[2]: https://travis-ci.org/anko/eslisp-camelify
[3]: https://gitter.im/anko/eslisp
[4]: https://www.npmjs.com/package/eslisp
[5]: test.esl
[6]: http://opensource.org/licenses/ISC
