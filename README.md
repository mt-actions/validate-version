# Validate Version Action

## Inputs
- comparison:
  - The kind of comparison to be done, where valid values are in the set { `>`, `<`, `==`, `>=`, `<=`, `!=` }
- left
- right


If `${left} ${comparison} ${right}` evaluates to false, the action will fail

## Examples:
- comparison: `>`
  - `${left} == ${right}` ==> FAIL
  - `${left} > ${right}` ==> PASS
  - `${left} < ${right}` ==> FAIL
- comparison: `<`
  - `${left} == ${right}` ==> FAIL
  - `${left} > ${right}` ==> FAIL
  - `${left} < ${right}` ==> PASS
- comparison: `==`
  - `${left} == ${right}` ==> PASS
  - `${left} > ${right}` ==> FAIL
  - `${left} < ${right}` ==> FAIL
- comparison: `>=`
  - `${left} == ${right}` ==> PASS
  - `${left} > ${right}` ==> PASS
  - `${left} < ${right}` ==> FAIL
- comparison: `<=`
  - `${left} == ${right}` ==> PASS
  - `${left} > ${right}` ==> FAIL
  - `${left} < ${right}` ==> PASS
- comparison: `!=`
  - `${left} == ${right}` ==> FAIL
  - `${left} > ${right}` ==> PASS
  - `${left} < ${right}` ==> PASS
