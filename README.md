# Interviewtopia household tax policy fixture

Static JSON fixtures for the second phase of the Interviewtopia frontend assessment.

- Swagger UI: <https://masseyis.github.io/interviewtopia-tax-policy-api/docs/>
- OpenAPI definition: <https://masseyis.github.io/interviewtopia-tax-policy-api/openapi.yaml>

The published endpoint pattern is:

```text
https://masseyis.github.io/interviewtopia-tax-policy-api/policies/{residents}.json
```

`residents` is an integer from 1 to 6. Each response describes the complete set of bands for that household size. Band order is deliberately not guaranteed.

Amounts are integer cents and rates are integer basis points. For example, `1000` basis points means 10%.

The calculator remains non-cumulative and rounds half up to the nearest cent. Those are fixed rules from the base exercise, not policy dimensions, so they are documented but are not properties in the response.

The endpoint is static and contains no personal, secret or production data.
