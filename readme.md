# eslisp-camelify [![](https://img.shields.io/travis/anko/eslisp-camelify.svg?style=flat-square)][1] [![](https://img.shields.io/badge/eslisp_chat-gitter_%E2%86%92-blue.svg?style=flat-square)][2]

An [eslisp][3] macro that rewrites all atoms in its arguments from
`dash-separated` to `camelCase`, but otherwise touches nothing.

Handy if you prefer lisp-like `dash-separated-variables`.

## Example

    (macro camelify (require "/path/to/eslisp-camelify/index.js"))
    (camelify (explain-that (the-answer-is 42)))

↓

    explainThat(theAnswerIs(42));

See [the tests][4] for fuller usage.

## License

[ISC][5].

[1]: https://travis-ci.org/anko/eslisp-camelify
[2]: https://gitter.im/anko/eslisp
[3]: https://www.npmjs.com/package/eslisp
[4]: test.esl
[5]: http://opensource.org/licenses/ISC
