# Free Historical WHOIS Data API

Access archived WHOIS records for any domain name through the WhoisDataCenter Historical WHOIS API.

See how a domain's WHOIS information changed over time, including past registrars, registrants, contact details, registration dates, expiry dates, name servers, and domain status.

## Endpoint

```http
GET https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical
```

## Parameters

| Parameter | Required | Description |
|---|---|---|
| domain | Yes | Domain name to look up, such as `marketxy.com` |
| format | No | Response format: `json`, `xml`, or `csv`. Default is `json` |

## Example Request

```bash
curl -X GET "https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical?domain=marketxy.com" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Accept: application/json"
```

## Get Your Free API Key

Create your free WhoisDataCenter account and get 10,000 free API credits.

https://app.whoisdatacenter.com/sign-up

## Authentication

Use your API key as a Bearer token:

```text
Authorization: Bearer YOUR_API_KEY
```

Never publish your real API key on GitHub or in public code.

## Example API URL

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical?domain=marketxy.com
```

## Response Formats

The API supports:

- JSON
- XML
- CSV

JSON is used by default.

### JSON

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical?domain=marketxy.com
```

### XML

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical?domain=marketxy.com&format=xml
```

### CSV

```text
https://api-v1.whoisdatacenter.com/api/v2/domain/whois/historical?domain=marketxy.com&format=csv
```

## Example JSON Response

```json
{
  "execution_time_ms": 2134,
  "status": true,
  "total_records": 9,
  "result_count": 9,
  "data": [
    {
      "domain_name": "marketxy.com",
      "query_time": "2026-05-12 11:27:03",
      "create_date": "2024-10-09",
      "update_date": "2025-07-12",
      "expiry_date": "2034-10-09",
      "domain_registrar_id": "1068",
      "domain_registrar_name": "NAMECHEAP INC",
      "domain_registrar_whois": "whois.namecheap.com",
      "domain_registrar_url": "http://www.namecheap.com",
      "registrant_name": "Redacted for Privacy",
      "registrant_company": "Privacy service provided by Withheld for Privacy ehf",
      "registrant_address": "Kalkofnsvegur 2",
      "registrant_city": "Reykjavik",
      "registrant_state": "Capital Region",
      "registrant_zip": "101",
      "registrant_country": "IS",
      "registrant_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
      "registrant_phone": "+354.4212434",
      "registrant_fax": "",
      "administrative_name": "Redacted for Privacy",
      "administrative_company": "Privacy service provided by Withheld for Privacy ehf",
      "administrative_address": "Kalkofnsvegur 2",
      "administrative_city": "Reykjavik",
      "administrative_state": "Capital Region",
      "administrative_zip": "101",
      "administrative_country": "IS",
      "administrative_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
      "administrative_phone": "+354.4212434",
      "administrative_fax": "",
      "technical_name": "Redacted for Privacy",
      "technical_company": "Privacy service provided by Withheld for Privacy ehf",
      "technical_address": "Kalkofnsvegur 2",
      "technical_city": "Reykjavik",
      "technical_state": "Capital Region",
      "technical_zip": "101",
      "technical_country": "IS",
      "technical_email": "226954c46487463d9eee2ab909daafd5.protect@withheldforprivacy.com",
      "technical_phone": "+354.4212434",
      "technical_fax": "",
      "billing_name": "",
      "billing_company": "",
      "billing_address": "",
      "billing_city": "",
      "billing_state": "",
      "billing_zip": "",
      "billing_country": "",
      "billing_email": "",
      "billing_phone": "",
      "billing_fax": "",
      "name_server_1": "cass.ns.cloudflare.com",
      "name_server_2": "gerald.ns.cloudflare.com",
      "name_server_3": "",
      "name_server_4": "",
      "domain_status_1": "clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
      "domain_status_2": "",
      "domain_status_3": "",
      "domain_status_4": ""
    },
    {
      "domain_name": "marketxy.com",
      "query_time": "2026-05-06 16:16:41",
      "create_date": "2024-10-09",
      "update_date": "2026-02-07",
      "expiry_date": "2034-10-09",
      "domain_registrar_id": "1068",
      "domain_registrar_name": "NameCheap; Inc.",
      "domain_registrar_whois": "",
      "domain_registrar_url": "http://www.namecheap.com",
      "registrant_name": "",
      "registrant_company": "",
      "registrant_address": "",
      "registrant_city": "",
      "registrant_state": "",
      "registrant_zip": "",
      "registrant_country": "",
      "registrant_email": "",
      "registrant_phone": "",
      "registrant_fax": "",
      "administrative_name": "",
      "administrative_company": "",
      "administrative_address": "",
      "administrative_city": "",
      "administrative_state": "",
      "administrative_zip": "",
      "administrative_country": "",
      "administrative_email": "",
      "administrative_phone": "",
      "administrative_fax": "",
      "technical_name": "",
      "technical_company": "",
      "technical_address": "",
      "technical_city": "",
      "technical_state": "",
      "technical_zip": "",
      "technical_country": "",
      "technical_email": "",
      "technical_phone": "",
      "technical_fax": "",
      "billing_name": "",
      "billing_company": "",
      "billing_address": "",
      "billing_city": "",
      "billing_state": "",
      "billing_zip": "",
      "billing_country": "",
      "billing_email": "",
      "billing_phone": "",
      "billing_fax": "",
      "name_server_1": "CASS.NS.CLOUDFLARE.COM",
      "name_server_2": "GERALD.NS.CLOUDFLARE.COM",
      "name_server_3": "",
      "name_server_4": "",
      "domain_status_1": "client transfer prohibited",
      "domain_status_2": "",
      "domain_status_3": "",
      "domain_status_4": ""
    }
  ]
}
```

The example above shows two historical records to keep the README easy to read. The real API response can return more records, depending on how much historical WHOIS data is available for the domain.

## Response Fields

| Field | Description |
|---|---|
| execution_time_ms | API execution time in milliseconds |
| status | Shows whether the API request was successful |
| total_records | Total number of historical WHOIS records found |
| result_count | Number of records returned in the response |
| data | Array containing historical WHOIS records |
| domain_name | Domain name |
| query_time | Date and time when the WHOIS record was collected |
| create_date | Domain creation date |
| update_date | Domain WHOIS update date |
| expiry_date | Domain expiration date |
| domain_registrar_name | Name of the domain registrar |
| domain_registrar_whois | Registrar WHOIS server |
| domain_registrar_url | Registrar website |
| registrant_name | Registrant name, when available |
| registrant_company | Registrant company or organization |
| registrant_country | Registrant country |
| registrant_email | Registrant email, when available |
| administrative_name | Administrative contact name |
| technical_name | Technical contact name |
| name_server_1 | Primary name server |
| name_server_2 | Secondary name server |
| domain_status_1 | Domain status |

Some WHOIS fields may be empty, redacted, hidden, or unavailable because of privacy protection, registry policies, or differences in historical records.

## What Historical WHOIS Data Can Show

Historical WHOIS data can help show changes in:

- Domain ownership
- Registrant name
- Registrant company
- Registrant email
- Registrant phone
- Domain registrar
- Creation date
- Expiry date
- Name servers
- Domain status
- Administrative contacts
- Technical contacts

## Use Cases

Historical WHOIS data can be used for:

- Cybersecurity investigations
- Threat intelligence
- OSINT research
- Domain ownership history
- Fraud investigations
- Brand protection
- Due diligence
- Legal research
- Domain portfolio research
- Tracking registrar changes
- Tracking nameserver changes
- Finding past domain owners

## Credits

Each Historical WHOIS lookup uses 5 API credits.

## For Support

https://whoisdatacenter.com/contact-us/

## Official Documentation

https://whoisdatacenter.com/api-docs/#historical-whois

## About WhoisDataCenter

WhoisDataCenter provides WHOIS data, historical WHOIS records, reverse WHOIS lookup, newly registered domain feeds, updated domain feeds, expired domains, expiring domains, dropped domains, and other domain intelligence APIs.

Website: https://whoisdatacenter.com
