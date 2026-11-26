# WholeCart – Test Execution Report

## Environment
- Application: WholeCart Marketplace
- Browser: Google Chrome
- Role: Buyer
- Account: buyer1

## Catalogue Test Results

| Test ID | Test Scenario | Test Data | Actual Result | Status |
|---|---|---|---|---|
| TC-001 | Search product using SKU | SKU-0471 | Correct product displayed | PASS |
| TC-002 | Search another product using SKU | SKU-0010 | Correct product displayed | PASS |
| TC-003 | Search using invalid SKU | INVALID99999 | No matching product displayed | PASS |
| TC-004 | Filter products by category | Grains | Grains products displayed | PASS |
| TC-005 | Combine SKU search and category filter | SKU-0471 + Grains | Snacks product displayed despite Grains filter | FAIL / Investigation required |

## Defect Reference

BUG-001 – Catalogue category filter behaviour during SKU search.

## Notes

The combined search and category filter behaviour requires confirmation against the intended filtering rules. Record the observed behaviour and clarify the requirement before treating it as a confirmed defect.
