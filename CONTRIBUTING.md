# Contributing

Thanks for taking a look. Each repository here is a small, dependency-free library behind one of the
free tools on [ExamineIP](https://tools.examineip.com/), maintained by one person.

## The most useful thing you can send: a wrong answer

These libraries exist because the usual tools get edge cases wrong. If you find an input where one of
them gives the wrong result, that is worth more than any feature:

1. Open an issue with the **exact input** (address, domain, header, record — whatever the library reads).
2. Say what it returned and what it **should** return.
3. Point to the evidence: the RFC section, a reference implementation's output, or a real-world record.

Please use documentation values where you can (`192.0.2.0/24`, `2001:db8::/32`, `example.com`) rather
than real people's addresses or domains.

## Pull requests

- **Keep it dependency-free.** Each library is a single file on purpose.
- **Add a test** to `tests/` that fails before your change and passes after it.
- **Match the style** of the file you are editing (the JS libraries are ES5-style with a UMD wrapper).
- **CI must pass** on every supported runtime listed in the workflow.
- Where an independent reference exists (Python's `ipaddress`, the platform's URL parser, an RFC test
  vector), test against it rather than against the library's own output.

Small, focused pull requests are easiest to review. For anything larger, open an issue first so we can
agree on the approach.

## Security problems

Do not open a public issue for a vulnerability — see [SECURITY.md](SECURITY.md).

## Conduct

By taking part you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).
