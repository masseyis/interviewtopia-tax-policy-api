# Interviewtopia household tax policy fixture

Static JSON fixtures for the second phase of the Interviewtopia frontend assessment.

The published endpoint pattern is:

```text
https://masseyis.github.io/interviewtopia-tax-policy-api/policies/{residents}.json
```

`residents` is an integer from 1 to 6. Each response describes a complete, non-cumulative tax policy. Band order is deliberately not guaranteed.

Amounts are integer pence and rates are integer basis points. For example, `1000` basis points means 10%.

The endpoint is static and contains no personal, secret or production data.
