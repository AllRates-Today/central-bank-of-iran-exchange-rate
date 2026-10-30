# Central Bank of Iran Exchange Rates API — central-bank-of-iran-exchange-rate

[![npm version](https://img.shields.io/npm/v/central-bank-of-iran-exchange-rate.svg)](https://www.npmjs.com/package/central-bank-of-iran-exchange-rate)
[![license](https://img.shields.io/npm/l/central-bank-of-iran-exchange-rate.svg)](https://github.com/AllRates-Today/central-bank-of-iran-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/central-bank-of-iran-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![USD/IRR today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fcbir%3Fsource%3DUSD%26target%3DIRR&query=%24.rate&label=USD%2FIRR%20published%20by%20Central%20Bank%20of%20Iran&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/cbir/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fcbir%3Fsource%3DUSD%26target%3DIRR&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/central-bank-rates-api/cbir/)

**Official Central Bank of Iran (Iran) daily exchange rates for Node.js and TypeScript. The published central bank rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers Central Bank of Iran itself prints, every business day.**

## 🚀 Why this client?

- 🏛️ **Official published rates** — Central Bank of Iran's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2002** — point-in-time tables and daily series for any past date
- 🔀 **Published vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number Central Bank of Iran itself published, fixed once printed and carrying the central bank's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest published table

[![Latest Central Bank of Iran table](https://allratestoday.com/api/open/central-bank/cbir/table.svg)](https://allratestoday.com/central-bank-rates-api/cbir/)

The image is rendered live from the keyless endpoint, so it follows the central bank's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the central bank publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-10-30 by Central Bank of Iran — 47 rates. Updated 2026-10-30.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| AED | IRR | reference | 508626 |
| AFN | IRR | reference | 28873 |
| AMD | IRR | reference | 5179.28 |
| AUD | IRR | reference | 1314352 |
| AZN | IRR | reference | 1098781 |
| BDT | IRR | reference | 15056.64 |
| BHD | IRR | reference | 4967894 |
| BYN | IRR | reference | 634810 |
| CAD | IRR | reference | 1330704 |
| CHF | IRR | reference | 2250118 |
| CNY | IRR | reference | 280201 |
| DKK | IRR | reference | 278401 |
| EUR | IRR | reference | 2080841 |
| GBP | IRR | reference | 2484633 |
| GEL | IRR | reference | 720152 |
| HKD | IRR | reference | 238093 |
| IDR | IRR | reference | 102.764 |
| INR | IRR | reference | 19607 |
| IQD | IRR | reference | 1232.72 |
| JOD | IRR | reference | 2634595 |
| JPY | IRR | reference | 11804.31 |
| KRW | IRR | reference | 1389.976 |
| KWD | IRR | reference | 5997833 |
| KZT | IRR | reference | 4103.14 |
| LKR | IRR | reference | 5621.8 |
| LYD | IRR | reference | 290441 |
| MMK | IRR | reference | 890 |
| MYR | IRR | reference | 458192 |
| NOK | IRR | reference | 201466 |
| NPR | IRR | reference | 12248.47 |
| NZD | IRR | reference | 1049910 |
| OMR | IRR | reference | 4854244 |
| PHP | IRR | reference | 29205.89 |
| PKR | IRR | reference | 6753.26 |
| QAR | IRR | reference | 513167 |
| RUB | IRR | reference | 23100 |
| SAR | IRR | reference | 498114 |
| SEK | IRR | reference | 188218 |
| SGD | IRR | reference | 1456101 |
| SYP | IRR | reference | 15308 |
| THB | IRR | reference | 55302.68 |
| TJS | IRR | reference | 202746 |
| TMT | IRR | reference | 533942 |
| TRY | IRR | reference | 37480 |
| USD | IRR | reference | 1867928 |
| VES | IRR | reference | 2106 |
| ZAR | IRR | reference | 112042 |

</details>

Source: [Official rates published by CBIR, served by AllRatesToday](https://allratestoday.com/central-bank-rates-api/cbir/). Rates are as printed by the central bank; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install central-bank-of-iran-exchange-rate
```

```bash
yarn add central-bank-of-iran-exchange-rate
```

```bash
pnpm add central-bank-of-iran-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/central-bank-of-iran-exchange-rate`](https://www.npmjs.com/package/@allratestoday/central-bank-of-iran-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'central-bank-of-iran-exchange-rate';

const pair = await getRate('USD', 'IRR', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official Central Bank of Iran rate, on the central bank's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest published table
- [Full published table](#full-published-table) — everything the central bank printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the central bank does not print directly are resolved from its table and flagged (see *Published vs derived rates* below).

```js
const pair = await getRate('USD', 'IRR', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'cbir',
  name: 'Central Bank of Iran',
  rate_date: '2026-10-20',   // Central Bank of Iran's own publication date
  source: 'USD',
  target: 'IRR',
  rate: 1832816,
  rate_type: 'reference',
  derived: false,
  method: 'published',
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full published table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'central-bank-of-iran-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'cbir',
  name: 'Central Bank of Iran',
  rate_date: '2026-10-20',
  rates: [
    { "base": "USD", "quote": "IRR", "type": "reference", "value": 1832816 },
    // … the rest of the published table (47 currencies vs IRR)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2002 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'central-bank-of-iran-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'IRR' });
```

**Response:**

```javascript
{
  bank: 'cbir',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'central-bank-of-iran-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'IRR', from: '2026-01-01', to: '2026-10-20' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'cbir',
  source: 'USD',
  target: 'IRR',
  from: '2026-01-01',
  to: '2026-10-20',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-10-20', rate: 1832816, rate_type: 'reference', derived: false, method: 'published' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

Central Bank of Iran currently publishes rates covering **47 currencies** against the IRR (as of the latest table):

🇦🇪 `AED` · 🇦🇫 `AFN` · 🇦🇲 `AMD` · 🇦🇺 `AUD` · 🇦🇿 `AZN` · 🇧🇩 `BDT` · 🇧🇭 `BHD` · 🇧🇾 `BYN` · 🇨🇦 `CAD` · 🇨🇭 `CHF` · 🇨🇳 `CNY` · 🇩🇰 `DKK` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇬🇪 `GEL` · 🇭🇰 `HKD` · 🇮🇩 `IDR` · 🇮🇳 `INR` · 🇮🇶 `IQD` · 🇯🇴 `JOD` · 🇯🇵 `JPY` · 🇰🇷 `KRW` · 🇰🇼 `KWD` · 🇰🇿 `KZT` · 🇱🇰 `LKR` · 🇱🇾 `LYD` · 🇲🇲 `MMK` · 🇲🇾 `MYR` · 🇳🇴 `NOK` · 🇳🇵 `NPR` · 🇳🇿 `NZD` · 🇴🇲 `OMR` · 🇵🇭 `PHP` · 🇵🇰 `PKR` · 🇶🇦 `QAR` · 🇷🇺 `RUB` · 🇸🇦 `SAR` · 🇸🇪 `SEK` · 🇸🇬 `SGD` · 🇸🇾 `SYP` · 🇹🇭 `THB` · 🇹🇯 `TJS` · 🇹🇲 `TMT` · 🇹🇷 `TRY` · 🇺🇸 `USD` · 🇻🇪 `VES` · 🇿🇦 `ZAR`

## 🏛️ Source

The Central Bank of the Islamic Republic of Iran publishes a daily table of exchange reference rates for the rial — 47 currencies in rials per unit, seven days a week, with the archive on the same page back to the March 2002 unification. The series carries Iran's exchange-rate history as the bank itself printed it: the 42,000-rial preferential rate from 2018 to late 2024, then a reference rate that tracks the market, which reached 1.8 million rials per dollar in October 2026. This is the bank's own table — not the open-market or exchange-house rate — and it is the rate Iranian customs, tax and accounting rules cite.

- Publisher's own page: [Exchange reference rates](https://www.cbi.ir/exrates/rates_en.aspx) · [www.cbi.ir](https://www.cbi.ir)
- Publication: every business day; the exact schedule, freshness status and any current delay are on the [Central Bank of Iran rates page](https://allratestoday.com/central-bank-rates-api/cbir/)
- In the API: usually by **19:20 UTC** (measured over the last 14 publications). Schedule a sync at or after that time and retry hourly until `rate_date` moves; every response carries the same figure as `available_by_utc` — see [when to poll](https://allratestoday.com/docs/#when-to-poll)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- Central Bank of Iran quotes **IRR per 1 unit of foreign currency** (e.g. `base: "USD", quote: "IRR"` means IRR per one US dollar).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the central bank's series a row belongs to (`reference` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official Central Bank of Iran rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/cbir/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('cbir')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate cbir ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Published vs derived rates

If Central Bank of Iran does not print a pair directly, the API resolves it from the central bank's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The central bank printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via IRR from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by Central Bank of Iran |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'central-bank-of-iran-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('central-bank-of-iran-exchange-rate');

getRate('USD', 'IRR', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once per business day — cache the published table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the published table |
| `getLatestRates({ apiKey })` | Free | The central bank's full latest published table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2002 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same published tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/cbir.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/cbir/latest.json`

## 🔗 Links

- [Central Bank of Iran rates page](https://allratestoday.com/central-bank-rates-api/cbir/) — live table, publication cadence, FAQ
- [All central bank sources](https://allratestoday.com/central-bank-rates-api/)
- [Package docs on the site](https://allratestoday.com/docs/sdk/central-bank-of-iran-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [GitHub](https://github.com/AllRates-Today/central-bank-of-iran-exchange-rate)

## 📜 License

MIT
