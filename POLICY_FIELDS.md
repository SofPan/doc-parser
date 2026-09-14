## Fields
- Policy Number: A unique ID code that the insurance company uses to track your specific account and paperwork.
- Named Insured: The official name of the person, family, or business that holds the insurance policy.
- Insurer Name: The official insurance company or carrier providing the financial coverage and backing.
- Effective/Expiry Dates: The start and end dates when the insurance policy is active and valid.
- Insured Item / Property: A description of the specific asset covered, such as a home address, a vehicle VIN, or business equipment.
- Coverage Limit: The maximum dollar amount the insurance company will pay out for a covered claim.
- Deductible: The specific out-of-pocket amount you must pay yourself before the insurance coverage starts paying.
- Premium: The total cost you pay to buy and keep the insurance policy active.
- Endorsements / Riders: A list of attached form numbers or special amendments that add, remove, or change standard policy rules.
- Additional Insured: A secondary person or business added to your policy for specific protections, commonly required in vendor or rental contracts.

## Field Extraction Rules
|          Field          |     Type     | Required? |       Define Valid     |    If missing    |
|-------------------------|--------------|-----------|------------------------|------------------|
| Policy Number           | String       | Yes       | Policy Identifier      | Flag review      |
| Named Insured           | String       | Yes       | Person/Business Name   | Flag review      |
| Insurer Name            | String       | Yes       | Carrier name           | Flag review      |
| Effective/Expiry Dates  | Date         | Yes       | Valid calendar dates   | Flag review      |
| Insured Item / Property | String       | Yes       | Description/identifier | Flag review      |
| Coverage Limit          | Currency     | Yes       | Monetary amount        | Flag review      |
| Deductible              | Currency     | Yes       | Monetary amount        | Flag review      |
| Premium                 | Currency     | Yes       | Monetary amount        | Flag review      |
| Endorsements / Riders   | Array        | No        | Form numbers/names     | Empty            |
| Additional Insured      | String/Array | No        | Named additional party | Empty            |