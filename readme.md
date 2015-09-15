# eslisp-camelify

An [eslisp][1] macro that rewrites all atoms in its arguments from
`dash-separated` to `camelCase`, but otherwise touches nothing.

Handy if you prefer using lisp-like `dash-separated-variables`, at
least for part of your code.

## Example

    (macro camelify (require "/path/to/eslisp-camelify/index.js"))
    (camelify (explain-that (the-answer-is 42)))

↓

    explainThat(theAnswerIs(42));

See [the tests][2] for fuller usage.

## License

[ISC][3].

[1]: https://www.npmjs.com/package/eslisp
[2]: test.esl
[3]: http://opensource.org/licenses/ISC
