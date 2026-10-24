# Reference
## reference
<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_sync</a>(...) -> ExchangeRatesSyncReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Fetches the euro exchange rates the Bank of Lithuania web service publishes for `date` (default: the company's current date) and stores them in the rate table shared by all companies, replacing the rates already stored for that date. Answers 404 when no rates are published for the date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.exchange_rates_sync()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_list</a>(...) -> ExchangeRatesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the stored euro exchange rates, which are shared by all companies. Filterable by `currencyCode` and `date`; sortable by `date` and `currencyCode`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.exchange_rates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ExchangeRatesListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ExchangeRatesListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_set</a>(...) -> ExchangeRatesSetReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stores a company exchange rate for `currency` on `date`, in units of the currency per one unit of the company's base currency, replacing the company rate stored for that currency and date. Rate lookups use the company rate when it is dated on or after the latest shared rate on or before the lookup date. Answers 422 when `rate` is not positive.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.exchange_rates_set(
    currency="currency",
    date=datetime.date.fromisoformat("2026-07-01"),
    rate="121.00000000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**currency:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**rate:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_overrides_list</a>(...) -> ExchangeRatesOverridesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's own exchange rates set with `reference/exchange-rates/set`. Filterable by `currencyCode` and `date`; sortable by `date` and `currencyCode`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.exchange_rates_overrides_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ExchangeRatesOverridesListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ExchangeRatesOverridesListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_overrides_delete</a>(...) -> ExchangeRatesOverridesDeleteReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the company's own exchange rate for `currency` on `date`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.exchange_rates_overrides_delete(
    currency="currency",
    date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**currency:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">countries_list</a>() -> CountriesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists every country code Nordlet knows with its EU and EEA membership and its name in each supported locale.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.countries_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">lt_counties_list</a>() -> LtCountiesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the ten Lithuanian counties (apskritys) with their code and ISO code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.lt_counties_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">lt_municipalities_list</a>(...) -> LtMunicipalitiesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the Lithuanian municipalities (savivaldybės) with the county each belongs to; `countyCode` limits the list to one county.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.lt_municipalities_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**county_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">lt_cities_list</a>(...) -> LtCitiesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists Lithuanian cities with their municipality; `municipalityCode` limits the list to one municipality and `q` to names that start with the given text (case-insensitive).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.lt_cities_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**municipality_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**q:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">banks_list</a>(...) -> BanksListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the banks of the bank directory shared by all companies. Filterable by `countryCode`, `name`, `bic` and `bankCode`; sortable by `name`, `bic` and `countryCode`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.banks_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[BanksListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[BanksListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">banks_upsert</a>(...) -> BanksUpsertReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a bank to the shared bank directory or, when a bank with the same `countryCode` and `bic` exists, replaces its name, bank code and active flag. Platform administrators only.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.banks_upsert(
    country_code="countryCode",
    name="name",
    bic="bic",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bank_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">lt_regions_list</a>() -> LtRegionsListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the ten Lithuanian regions (apskritys) with their code and ISO code; the same list as `reference/lt/counties/list`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.lt_regions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">currencies_list</a>(...) -> CurrenciesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the currencies known to Nordlet with their minor units. Filterable and sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.currencies_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[CurrenciesListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[CurrenciesListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">vat_classifiers_list</a>(...) -> VatClassifiersListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's VAT classifiers (code, country, name and rate). A document line that names a classifier in `vatClassifierCode` takes its rate from it when neither the line nor the item has a rate. Filterable by `code`, `countryCode` and `ratePercent`; sortable by `code` and `ratePercent`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.vat_classifiers_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[VatClassifiersListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[VatClassifiersListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">vat_classifiers_upsert</a>(...) -> VatClassifiersUpsertReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds VAT classifiers to the company or replaces the country, name and rate of the ones whose `code` already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.reference import VatClassifiersUpsertReferenceRequestRowsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.vat_classifiers_upsert(
    rows=[
        VatClassifiersUpsertReferenceRequestRowsItem(
            code="code",
            name="name",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**rows:** `typing.List[VatClassifiersUpsertReferenceRequestRowsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">eu_vat_rates_list</a>(...) -> EuVatRatesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Effective EU VAT rate mapping for this company: EC TEDB defaults, replaced per country by any company overrides. Verify the mapping fits the goods and services you sell before relying on it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.eu_vat_rates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">eu_vat_rates_set_overrides</a>(...) -> EuVatRatesSetOverridesReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replace the VAT rate mapping this company uses for one EU country. Pass an empty rates array to drop the overrides and return to the TEDB defaults. Overrides feed rate suggestions (vat/resolve) and OSS/IOSS return rate classification.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.reference import EuVatRatesSetOverridesReferenceRequestRatesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.eu_vat_rates_set_overrides(
    country_code="countryCode",
    rates=[
        EuVatRatesSetOverridesReferenceRequestRatesItem(
            category="standard",
            rate_percent="121.00",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**rates:** `typing.List[EuVatRatesSetOverridesReferenceRequestRatesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">vat_resolve</a>(...) -> VatResolveReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Works out the VAT treatment of a supply by this company: the scheme (domestic, intra-EU B2B, reverse charge, OSS, IOSS, marketplace deemed supplier, export, out of scope or SME exempt), the country whose VAT applies, its rates with the company's overrides applied, and the legal basis. The customer comes from `partnerId` (country from the partner's address or VAT number, business status from the VAT number) or from `customerCountryCode` and `customerIsBusiness`; `date` defaults to the company's current date; when `belowDistanceSalesThreshold` is not given, the distance-sales threshold is tracked from the company's ledger. Answers 422 when the partner has neither an address country nor a VAT code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.vat_resolve()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**customer_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**customer_is_business:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**supply_type:** `typing.Optional[VatResolveReferenceRequestSupplyType]` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**below_distance_sales_threshold:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**facilitated_by_marketplace:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**acting_as_marketplace:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**seller_established_in_eu:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**imported_consignment_value_eur:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**service_kind:** `typing.Optional[VatResolveReferenceRequestServiceKind]` 
    
</dd>
</dl>

<dl>
<dd>

**service_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**underlying_supplier_gave_vat_number:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**underlying_supplier_charges_vat:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**goods_kind:** `typing.Optional[VatResolveReferenceRequestGoodsKind]` 
    
</dd>
</dl>

<dl>
<dd>

**goods_location_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">cn_codes_list</a>(...) -> CnCodesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the Combined Nomenclature codes of the directory shared by all companies. Filterable by `code`, `name` and `nameLt`; sortable by `code`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.cn_codes_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[CnCodesListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[CnCodesListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">cn_codes_upsert</a>(...) -> CnCodesUpsertReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds Combined Nomenclature codes to the shared directory or replaces the names and supplementary unit of the codes that exist. Platform administrators only.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.reference import CnCodesUpsertReferenceRequestRowsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.cn_codes_upsert(
    rows=[
        CnCodesUpsertReferenceRequestRowsItem(
            code="code",
            name="name",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**rows:** `typing.List[CnCodesUpsertReferenceRequestRowsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">compliance_versions_list</a>(...) -> ComplianceVersionsListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the versions of the filing systems, schemas and forms Nordlet's output was checked against, with the date of the check and the source; `country` limits the list to one country.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.compliance_versions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">intrastat_thresholds_list</a>() -> IntrastatThresholdsListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the Intrastat thresholds stored per year: the reporting and the statistical-value threshold for arrivals and for dispatches.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.intrastat_thresholds_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">units_list</a>(...) -> UnitsListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the measurement units of the directory shared by all companies, with Lithuanian and English names. Filterable by `code`, `nameLt` and `nameEn`; sortable by `code`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.units_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[UnitsListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[UnitsListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">series_create</a>(...) -> SeriesCreateReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a numbering series for a document type, prefix and year; the first number the series hands out is at least `startAt`. Answers 409 when a series with the same document type, prefix and year exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.series_create(
    document_type="documentType",
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**document_type:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**prefix:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**start_at:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">series_list</a>(...) -> SeriesListReferenceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's numbering series with the next number of each. Filterable and sortable by `documentType`, `prefix` and `year`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.series_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SeriesListReferenceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SeriesListReferenceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## partners
<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">addresses_create</a>(...) -> AddressesCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds an address of type billing, shipping, registered or other to the partner in `partnerId`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.addresses_create(
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[AddressesCreatePartnersRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**street:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**city:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**postal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">addresses_update</a>(...) -> AddressesUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of a partner address.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.addresses_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[AddressesUpdatePartnersRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**street:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**city:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**postal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">addresses_delete</a>(...) -> AddressesDeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a partner address.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.addresses_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">addresses_list</a>(...) -> AddressesListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists partner addresses; filterable by `partnerId`, `type` and `city`, sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.addresses_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AddressesListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AddressesListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">contacts_create</a>(...) -> ContactsCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a contact person to the partner in `partnerId`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.contacts_create(
    name="name",
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">contacts_update</a>(...) -> ContactsUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of a partner contact.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.contacts_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">contacts_delete</a>(...) -> ContactsDeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a partner contact.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.contacts_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">contacts_list</a>(...) -> ContactsListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists partner contacts; filterable by `partnerId`, `name` and `email`, sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.contacts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ContactsListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ContactsListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">bank_accounts_create</a>(...) -> BankAccountsCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a bank account to the partner in `partnerId`. The IBAN is stored without spaces in upper case; an IBAN the partner already has is refused with 409. With `isDefault` true the partner's other accounts lose their default mark.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.bank_accounts_create(
    iban="iban",
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**iban:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bank_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">bank_accounts_update</a>(...) -> BankAccountsUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of a partner bank account. A new IBAN is stored without spaces in upper case and is refused with 409 when the partner already has it; when the account is the default after the change, the partner's other accounts lose their default mark.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.bank_accounts_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">bank_accounts_delete</a>(...) -> BankAccountsDeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a partner bank account.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.bank_accounts_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">bank_accounts_list</a>(...) -> BankAccountsListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists partner bank accounts; filterable by `partnerId` and `iban`, sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.bank_accounts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[BankAccountsListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[BankAccountsListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">files_list</a>(...) -> FilesListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the files attached to a partner, newest first. `partners/create` attaches one with `documentRef`, and `leads/convert` moves the lead's files here.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.files_list(
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">debt_reminders_preview</a>() -> DebtRemindersPreviewPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Runs the overdue selection of the daily debt-reminder job for this company as of the company's current date and returns the overdue reminders it would send, without sending or recording anything. A partner is included when it has `autoDebtReminder`, is active, has an e-mail address, got no overdue reminder in the last `repeatDays` days (`partners/debt-reminders/settings/get`) and has issued invoices or advance invoices past their due date with an unpaid remainder; the interest per invoice is the remainder times the partner's `lateInterestPercent` times the days late over 365, and the totals are per currency. Sent reminders are listed by `partners/debt-reminders/list`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.debt_reminders_preview()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">debt_reminders_list</a>(...) -> DebtRemindersListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the debt reminders the daily job has sent, one row per partner and currency with the ids of the invoices it covered and its `kind` (`before_due` or `overdue`); filterable by `partnerId`, sortable by `sentAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.debt_reminders_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DebtRemindersListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DebtRemindersListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">debt_reminders_settings_get</a>() -> DebtRemindersSettingsGetPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the debt-reminder schedule of the company: `daysBefore`, the days before the due date on which the first reminder is sent (null when no reminder is sent before the due date), and `repeatDays`, the days between overdue reminders to a partner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.debt_reminders_settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">debt_reminders_settings_update</a>(...) -> DebtRemindersSettingsUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of the company's debt-reminder schedule. `daysBefore` (1 to 90, or null to send nothing before the due date) makes the daily job send one "payment due soon" reminder per invoice that many days before its due date; `repeatDays` (1 to 90) is the number of days between overdue reminders to a partner. Only partners with `autoDebtReminder` get reminders. A body without fields is refused with 400.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.debt_reminders_settings_update()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**days_before:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**repeat_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">debt_reminders_upcoming</a>() -> DebtRemindersUpcomingPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the next reminder the daily debt-reminder job would send for each unpaid issued invoice or advance invoice of the partners that get reminders (`autoDebtReminder`, active, with an e-mail address), as of the company's current date and sorted by `date`. A `before_due` reminder is sent once per invoice, `daysBefore` days before its due date or on the first daily run after that while the due date is still ahead; `overdue` reminders start the day after the due date and repeat every `repeatDays` days per partner, counting only overdue reminders. Nothing is sent or recorded.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.debt_reminders_upcoming()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">validate_vat</a>(...) -> ValidateVatPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Checks a VAT number against VIES, either a free `vatCode` or the VAT code of the partner in `partnerId` (exactly one of the two); a code without an EU country prefix and 2 to 12 alphanumeric characters is refused with 422, as is a partner without a VAT code, and a VIES outage answers 503. With a partner the outcome is written to it (`vatValid`, `vatValidatedAt`): an invalid number or a VIES name that shares no word with the partner's name opens or refreshes the partner's VAT review (`vat_review.opened`), a VIES failure opens one with reason `service_error`, and a valid matching number resolves the open review as `revalidated` (`vat_review.resolved`). Reviews are listed and closed with `partners/vat-reviews/list` and `partners/vat-reviews/resolve`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.validate_vat()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">vat_reviews_list</a>(...) -> VatReviewsListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the VAT reviews opened by VIES checks of partners' VAT codes, with reason `invalid`, `name_mismatch` or `service_error`; filterable by `partnerId`, `status` and `reason`, sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.vat_reviews_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[VatReviewsListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[VatReviewsListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">vat_reviews_resolve</a>(...) -> VatReviewsResolvePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Closes an open VAT review as `confirmed_valid`, `confirmed_invalid` or `dismissed`, with an optional note. The first two also set the partner's `vatValid` and stamp `vatValidatedAt` when the partner still carries the reviewed VAT code; `dismissed` leaves the partner unchanged. A review that is already resolved answers 409; emits `vat_review.resolved`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.vat_reviews_resolve(
    id="id",
    resolution="confirmed_valid",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**resolution:** `VatReviewsResolvePartnersRequestResolution` 
    
</dd>
</dl>

<dl>
<dd>

**note:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">create</a>(...) -> CreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a partner. `groupId`, `statusId` and `priceListId` must belong to the company; without `legalCountryClass` the class is derived from the address country (`lt`, `eu` or `non_eu`); `documentRef` attaches an uploaded file that is not yet linked to a record; a `code` already used by a live partner of the company is refused with 409. A `vatCode` is checked against VIES at once and the result stored on the partner: an invalid number, a VIES name that shares no word with the partner's name, or a VIES failure opens a VAT review (`vat_review.opened`), while a code that is not an EU VAT number is stored unchecked (see `partners/validate-vat`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[CreatePartnersRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**peppol_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**self_employment_cert_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**is_customer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_supplier:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_term_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**credit_limit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_list_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[CreatePartnersRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[CreatePartnersRequestCorrespondenceAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**short_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fax:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**eori_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_debt_reminder:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**late_interest_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**rating:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_employee:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_group_member:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**legal_country_class:** `typing.Optional[CreatePartnersRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">find_or_create</a>(...) -> FindOrCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the live partner matched by `code`, then `vatCode`, then `email` (at least one is required), or creates one from the body with the same validation and VIES check as `partners/create`; `created` says which happened. A creation that loses a race on the partner code returns the partner the other call created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.find_or_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[FindOrCreatePartnersRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**peppol_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**self_employment_cert_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**is_customer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_supplier:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_term_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**credit_limit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_list_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[FindOrCreatePartnersRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[FindOrCreatePartnersRequestCorrespondenceAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**short_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fax:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**eori_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_debt_reminder:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**late_interest_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**rating:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_employee:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_group_member:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**legal_country_class:** `typing.Optional[FindOrCreatePartnersRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">get</a>(...) -> GetPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns one partner; a deleted partner answers 404.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">update</a>(...) -> UpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of a partner; the clearable fields accept null. A new address country re-derives `legalCountryClass` unless the class is given, and a `code` already used by another live partner of the company is refused with 409. A changed `vatCode` resets the VIES result and is checked at once as in `partners/create`; a removed code, or one that is not an EU VAT number, resolves the partner's open VAT review as `superseded` (`vat_review.resolved`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[UpdatePartnersRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**peppol_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**self_employment_cert_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**is_customer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_supplier:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_term_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**credit_limit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_list_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[UpdatePartnersRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[UpdatePartnersRequestCorrespondenceAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**short_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fax:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**eori_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_debt_reminder:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**late_interest_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**rating:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_employee:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_group_member:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**legal_country_class:** `typing.Optional[UpdatePartnersRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">delete</a>(...) -> DeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Marks a partner as deleted; it no longer appears in lists or lookups.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">merge</a>(...) -> MergePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Moves every row that references the duplicate `sourceId` through a foreign key to partners (looked up in the database catalogue, within the company) to `targetId`, then marks the source partner as deleted; `moved` lists the tables, columns and row counts. Merging a partner into itself is 422, and when both partners hold the same unique entry (for example the same IBAN or item supplier row) the merge is refused with 409 until it is removed from one of them. When the kept partner has an open VAT review, the duplicate's open review is resolved as `superseded` (`vat_review.resolved`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.merge(
    source_id="sourceId",
    target_id="targetId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**source_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**target_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">anonymize</a>(...) -> AnonymizePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes birth date, self-employment certificate number, email, phone, address, notes, contacts, addresses and bank accounts, then hides the partner. The name, code and VAT number stay because issued invoices must keep identifying the counterparty for the statutory retention period.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.anonymize(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">list</a>(...) -> ListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists live partners; filterable by `name`, `code`, `vatCode`, `email`, `type`, `isCustomer`, `isSupplier`, `isActive`, `legalCountryClass`, `isEmployee`, `groupId`, `statusId` and `nextCallDate`, sortable by `name`, `code`, `createdAt`, `nextCallDate` and `rating`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">groups_create</a>(...) -> GroupsCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a partner group; a `code` already used by a group of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.groups_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">groups_update</a>(...) -> GroupsUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the code or name of a partner group; a code already used by another group of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.groups_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">groups_delete</a>(...) -> GroupsDeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a partner group; a group still assigned to a live partner is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.groups_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">groups_list</a>() -> GroupsListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's partner groups ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.groups_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">statuses_create</a>(...) -> StatusesCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a partner status with a `sortOrder`; a `code` already used by a status of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.statuses_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">statuses_update</a>(...) -> StatusesUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the code, name or sort order of a partner status; a code already used by another status of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.statuses_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">statuses_delete</a>(...) -> StatusesDeletePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a partner status; a status still assigned to a live partner is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.statuses_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">statuses_list</a>() -> StatusesListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's partner statuses ordered by sort order, then code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.statuses_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">inquiries_create</a>(...) -> InquiriesCreatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Records an inquiry in status `new`, from a partner (`partnerId`) or from a contact given by `contactName` or `contactEmail`; without any of the three it is refused with 422. `assignedUserId` must be a member of the company. Emits `partner_inquiry.created`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.inquiries_create(
    subject="subject",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**subject:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**contact_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**contact_email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**contact_phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**body:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**channel:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**assigned_user_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">inquiries_update</a>(...) -> InquiriesUpdatePartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of an inquiry; `partnerId` and `assignedUserId` accept null. Setting `status` to `closed` stamps `closedAt`, and moving a closed inquiry to another status clears it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.inquiries_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**subject:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**body:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**channel:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[InquiriesUpdatePartnersRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**assigned_user_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">inquiries_get</a>(...) -> InquiriesGetPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns one inquiry with the name of its partner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.inquiries_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">inquiries_list</a>(...) -> InquiriesListPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists inquiries with their partner names; filterable by `status`, `channel`, `partnerId`, `assignedUserId` and `subject`, sortable by `createdAt` and `updatedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.inquiries_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[InquiriesListPartnersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[InquiriesListPartnersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">credit_check</a>(...) -> CreditCheckPartnersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compares a partner's open receivables plus an optional `additionalAmount` with its `creditLimit`. The open receivables are the unpaid remainder of the partner's issued invoices, advance invoices and credit notes (credit notes negative), converted to the company's base currency at each invoice's `fxRate`. Without a credit limit `available` is null and `exceeded` is false.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.credit_check(
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**additional_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Leads
<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">create</a>(...) -> CreateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a lead in status `new`, `contacted`, `qualified` or `lost`. `assignedUserId` must be a member of the company and `sourceId` and `typeId` must exist in it; `countryCode` and `currency` are stored in upper case; `documents` attach uploaded files not yet linked to a record, and `notes` become the lead's first notes with the caller as author. Emits `lead.created`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**contact_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**source_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[CreateLeadsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**estimated_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**assigned_user_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[CreateLeadsRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">get</a>(...) -> GetLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns one lead with its source and type names.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">update</a>(...) -> UpdateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of a lead; the clearable fields accept null, `documents` attach more uploaded files, and `countryCode` and `currency` are stored in upper case. A lead that is already converted cannot change `status` (409).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**contact_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**source_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[UpdateLeadsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**estimated_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**assigned_user_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[UpdateLeadsRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">delete</a>(...) -> DeleteLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a lead with its notes and detaches its files, which stay in the company's files without a record.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">list</a>(...) -> ListLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists leads with their source and type names; filterable by `name`, `contactName`, `email`, `phone`, `status`, `sourceId`, `typeId`, `countryCode`, `assignedUserId`, `partnerId`, `estimatedValue` and `createdAt`, sortable by `name`, `status`, `estimatedValue`, `createdAt` and `updatedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListLeadsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListLeadsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">notes_create</a>(...) -> NotesCreateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a note to a lead with the caller as author and refreshes the lead's `updatedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.notes_create(
    lead_id="leadId",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**lead_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">notes_delete</a>(...) -> NotesDeleteLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a lead note.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.notes_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">notes_list</a>(...) -> NotesListLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the notes of a lead, newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.notes_list(
    lead_id="leadId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**lead_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">files_list</a>(...) -> FilesListLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the files attached to a lead, newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.files_list(
    lead_id="leadId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**lead_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">sources_create</a>(...) -> SourcesCreateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a lead source; a `name` already used by a source of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.sources_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">sources_update</a>(...) -> SourcesUpdateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the name or `isActive` flag of a lead source; a name already used by another source of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.sources_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">sources_delete</a>(...) -> SourcesDeleteLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a lead source; one still referenced by a lead is refused with 409 and should be deactivated with `leads/sources/update` instead.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.sources_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">sources_list</a>() -> SourcesListLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists all lead sources of the company, active and inactive, ordered by name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.sources_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">sources_options</a>() -> SourcesOptionsLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the id and name of the active lead sources, ordered by name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.sources_options()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">types_create</a>(...) -> TypesCreateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a lead type; a `name` already used by a type of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.types_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">types_update</a>(...) -> TypesUpdateLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the name or `isActive` flag of a lead type; a name already used by another type of the company is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.types_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">types_delete</a>(...) -> TypesDeleteLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a lead type; one still referenced by a lead is refused with 409 and should be deactivated with `leads/types/update` instead.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.types_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">types_list</a>() -> TypesListLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists all lead types of the company, active and inactive, ordered by name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.types_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">types_options</a>() -> TypesOptionsLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the id and name of the active lead types, ordered by name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.types_options()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.leads.<a href="src/nordlet/leads/client.py">convert</a>(...) -> ConvertLeadsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a customer partner from the lead, move the lead files to the partner, copy the lead notes into the partner notes and mark the lead as converted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.leads.convert(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_type:** `typing.Optional[ConvertLeadsRequestPartnerType]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## catalog
<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_create</a>(...) -> ItemsCreateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a catalog item: a product, a service or a set of other items. `unit` must be `vnt`, a global measurement unit or one of the company's own units (`catalog/units/options`), the sale, purchase and expense account codes must be postable accounts of the chart, and `priceFrom`/`priceTo` and `validFrom`/`validTo` must be in order; otherwise 422. A `set` needs at least one component and none of them may be a set; `components` on any other type is refused with 422. 409 when an active item already carries the `code`. `documentRef` is the storage key of a file uploaded with `files/upload`, which is attached to the item. Emits `item.created`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ItemsCreateCatalogRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**tracking:** `typing.Optional[ItemsCreateCatalogRequestTracking]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**barcode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_classifier_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_price_excl_vat:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_price_excl_vat:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cn_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**origin_country:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**net_mass_kg:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_qty_per_unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**translations:** `typing.Optional[typing.Dict[str, ItemsCreateCatalogRequestTranslationsValue]]` 
    
</dd>
</dl>

<dl>
<dd>

**components:** `typing.Optional[typing.List[ItemsCreateCatalogRequestComponentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**kind_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**manufacturer:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**gross_mass_kg:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**min_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost_price:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_free_price:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**external_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_returnable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**comment_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**price_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**price_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**min_price:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**max_discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**loyalty_points:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**department:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**age_restriction:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**package_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tara_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**certificate_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**certificate_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**pos_flags:** `typing.Optional[typing.Dict[str, bool]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_get</a>(...) -> ItemsGetCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one item; a set comes with its components.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_update</a>(...) -> ItemsUpdateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the fields of an item; the fields that are nullable in the request can be set to null to clear them. The checks of `catalog/items/create` apply. `components` replaces the whole component list and is accepted only when the item is or becomes a set (422); turning an item into a set needs components and is refused with 409 while the item is itself a component of another set. Turning a set into another type removes its components. 409 when an active item already carries the new `code`. Emits `item.updated`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ItemsUpdateCatalogRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**tracking:** `typing.Optional[ItemsUpdateCatalogRequestTracking]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**barcode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_classifier_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_price_excl_vat:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_price_excl_vat:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cn_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**origin_country:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**net_mass_kg:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_qty_per_unit:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.Dict[str, typing.Optional[str]]]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**translations:** `typing.Optional[typing.Dict[str, typing.Optional[ItemsUpdateCatalogRequestTranslationsValue]]]` 
    
</dd>
</dl>

<dl>
<dd>

**components:** `typing.Optional[typing.List[ItemsUpdateCatalogRequestComponentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**kind_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**manufacturer:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**gross_mass_kg:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**min_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost_price:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_free_price:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**external_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_returnable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**comment_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**price_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**price_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**min_price:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**max_discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**loyalty_points:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**department:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**age_restriction:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**package_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tara_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**certificate_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**certificate_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**pos_flags:** `typing.Optional[typing.Dict[str, typing.Optional[bool]]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_delete</a>(...) -> ItemsDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Soft-delete an item. Refused with 409 while the item is a component of an active set. Emits `item.deleted`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_list</a>(...) -> ItemsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the active items. Filterable: name, code, barcode, type, vatClassifierCode, groupId, kindId, externalId, manufacturer, department. Sortable: name, code, createdAt, updatedAt, salePriceExclVat; default name ascending. Rows carry no components; `catalog/items/get` returns them.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ItemsListCatalogRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ItemsListCatalogRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_files_list</a>(...) -> ItemsFilesListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the files attached to an item, newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_files_list(
    item_id="itemId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_kinds_create</a>(...) -> ItemsKindsCreateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an item kind: a code, a name, the SAF-T item type, whether quantities are accounted for, and a sort order. 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_kinds_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**saft_type:** `typing.Optional[ItemsKindsCreateCatalogRequestSaftType]` 
    
</dd>
</dl>

<dl>
<dd>

**quantity_accounting:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_kinds_update</a>(...) -> ItemsKindsUpdateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change an item kind. 409 when the new code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_kinds_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**saft_type:** `typing.Optional[ItemsKindsUpdateCatalogRequestSaftType]` 
    
</dd>
</dl>

<dl>
<dd>

**quantity_accounting:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_kinds_delete</a>(...) -> ItemsKindsDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete an item kind. Refused with 409 while an active item uses it; soft-deleted items that still carry it are detached.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_kinds_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_kinds_list</a>() -> ItemsKindsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's item kinds in sort order, then by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_kinds_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">units_create</a>(...) -> UnitsCreateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a unit of measure of the company's own, in addition to the global measurement units (`reference/units/list`). 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.units_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">units_update</a>(...) -> UnitsUpdateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the code, name or active flag of a company unit. 409 when the new code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.units_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">units_delete</a>(...) -> UnitsDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a company unit of measure.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.units_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">units_list</a>() -> UnitsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's own units of measure, ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.units_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">units_options</a>(...) -> UnitsOptionsCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the unit codes an item can use: the company's active own units first, then the global measurement units, named in the requested `locale` (Lithuanian for `lt`, English otherwise). A company unit hides a global unit with the same code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.units_options()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `typing.Optional[UnitsOptionsCatalogRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">item_groups_create</a>(...) -> ItemGroupsCreateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an item group, optionally under `parentId`. 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.item_groups_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">item_groups_update</a>(...) -> ItemGroupsUpdateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the code, name or parent of an item group; `parentId` null moves it to the top level. 422 when the new parent is the group itself or one of its descendants. 409 when the new code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.item_groups_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">item_groups_delete</a>(...) -> ItemGroupsDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete an item group. Refused with 409 while it has child groups or active items assigned.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.item_groups_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">item_groups_list</a>() -> ItemGroupsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's item groups, ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.item_groups_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_suppliers_upsert</a>(...) -> ItemsSuppliersUpsertCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create or replace the supplier record of an item for a partner (one per item and partner): supplier code, purchase price excluding VAT, currency (EUR when omitted) and notes. Fields omitted from the request are cleared on an existing record.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_suppliers_upsert(
    item_id="itemId",
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**supplier_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_price_excl_vat:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_suppliers_list</a>(...) -> ItemsSuppliersListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the supplier records, optionally for one `itemId` and/or `partnerId`, ordered by partner name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_suppliers_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">items_suppliers_delete</a>(...) -> ItemsSuppliersDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete the supplier record of an item.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.items_suppliers_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_create</a>(...) -> PriceListsCreateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a price list (currency EUR and active when omitted). 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_update</a>(...) -> PriceListsUpdateCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a price list. 409 when the new code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_list</a>() -> PriceListsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's price lists, ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_items_set</a>(...) -> PriceListsItemsSetCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the unit price excluding VAT of up to 500 items on a price list; a price already on the list is replaced and the other items on the list are kept. 422 when an item appears twice in the request. Emits `price_list.updated` with the item ids.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.catalog import PriceListsItemsSetCatalogRequestItemsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_items_set(
    price_list_id="priceListId",
    items=[
        PriceListsItemsSetCatalogRequestItemsItem(
            item_id="itemId",
            unit_price_excl_vat="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**price_list_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.List[PriceListsItemsSetCatalogRequestItemsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_items_list</a>(...) -> PriceListsItemsListCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the prices of a price list with the item name and code, ordered by item name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_items_list(
    price_list_id="priceListId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**price_list_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">price_lists_items_delete</a>(...) -> PriceListsItemsDeleteCatalogResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove one item from a price list.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.price_lists_items_delete(
    price_list_id="priceListId",
    item_id="itemId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**price_list_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## sales
<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_create</a>(...) -> InvoicesCreateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft sale document - an invoice, credit note, proforma or advance invoice (`type`) - with its lines; the totals are computed from the lines and `discountPercent`, and the number is assigned by `sales/invoices/issue`. Answers 422 when a credit note credits a proforma, another credit note or a document that is not issued, when the credited document has another partner or currency, when an OSS or IOSS document has no EU `vatCountryCode`, when the lines carry VAT but the company is not a VAT payer or the VAT scheme charges none, or when the operation type or document series is for another document type.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.sales import InvoicesCreateSalesRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_create(
    partner_id="partnerId",
    lines=[
        InvoicesCreateSalesRequestLinesItem()
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[InvoicesCreateSalesRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[InvoicesCreateSalesRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**credited_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**credited_invoice_reference:** `typing.Optional[str]` — Number of an original invoice issued outside Nordlet; give it with creditedInvoiceDate
    
</dd>
</dl>

<dl>
<dd>

**credited_invoice_date:** `typing.Optional[datetime.date]` — Issue date of the original invoice issued outside Nordlet
    
</dd>
</dl>

<dl>
<dd>

**agreement_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[InvoicesCreateSalesRequestVatScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**deemed_supplier:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvoicesCreateSalesRequestLocale]` — Language of the PDF and of the e-mail the invoice is sent with; unset means the language asked for when the PDF is made
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_series_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_get</a>(...) -> InvoicesGetSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one sale document with its lines, its VAT evidence and, on an advance invoice, the gross amount already applied to final invoices.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_pdf</a>(...) -> InvoicesPdfSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render a sale document, draft or issued, as a PDF returned base64-encoded. The document's own `locale` wins over the requested one. When the company has a payment link template and the document is issued and not paid, the PDF carries the payment link.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_pdf(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvoicesPdfSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_send</a>(...) -> InvoicesSendSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

E-mail an issued sale document as a PDF attachment to `to`, else to the partner's e-mail address, and emit `sale_invoice.sent`. The PDF is the one of `sales/invoices/pdf`. Answers 422 when e-mail sending is not configured, when the document is not issued, or when neither `to` nor the partner's e-mail is set.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_send(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvoicesSendSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_peppol_xml</a>(...) -> InvoicesPeppolXmlSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render an issued invoice or credit note as a Peppol BIS Billing 3.0 UBL file, returned base64-encoded with the sender and receiver participant identifiers, without sending it; `sales/invoices/peppol-send` sends the same file. Answers 422 for a draft, a proforma or an advance invoice.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_peppol_xml(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_peppol_send</a>(...) -> InvoicesPeppolSendSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send an issued invoice or credit note to the customer over Peppol through the company's own access point (Account → Compliance → EU; Nordlet supports Recommand, Storecove and e-invoice.be). Without one the call is refused with 422 and the document can only be downloaded with `sales/invoices/peppol-xml`. `status` is `pending` until the receiving access point confirms, then `delivered`; `failed` and `rejected` come with `detail`, and the invoice can then be sent again. Later changes arrive through the access point's webhook and are announced as `sale_invoice.peppol_delivered`, `sale_invoice.peppol_rejected` and `sale_invoice.peppol_failed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_peppol_send(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_peppol_status</a>(...) -> InvoicesPeppolStatusSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Ask the company's Peppol access point what happened to an invoice sent with `sales/invoices/peppol-send`, and store the answer: `pending`, `delivered` (the receiving access point confirmed it), `rejected` (the receiver refused it, see `detail`) or `failed` (it could not be delivered, see `detail`). The access point's webhook updates the same fields without this call. Storecove has no call for the status of a sent document, so for a Storecove access point this answers 422 and the status comes only from its webhook.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_peppol_status(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_einvoice_xml</a>(...) -> InvoicesEinvoiceXmlSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render an issued invoice as the national e-invoicing payload for the company country: FatturaPA (IT), KSeF FA(3) (PL) or UBL CIUS-RO (RO). Review the warnings - data the invoice does not carry is flagged, never invented.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_einvoice_xml(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_einvoice_send</a>(...) -> InvoicesEinvoiceSendSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the national e-invoicing payload and deliver it over the transport configured for the country gateway in compliance settings. With transport=direct the request talks to the tax authority itself - SdICoop over 2-way TLS for Italy, a KSeF session for Poland, ANAF SPV OAuth for Romania - and returns the national number as soon as the channel assigns one. With transport=bridge the payload goes to the configured bridge endpoint (an accredited intermediary or connector) instead.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_einvoice_send(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_einvoice_status</a>(...) -> InvoicesEinvoiceStatusSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Ask the national e-invoicing channel what happened to an invoice that was already sent, and store the answer. Italy, Poland and Romania return the outcome only on request - none of them calls back - so this is the way the national number and any rejection reason reach the invoice.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_einvoice_status(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_update</a>(...) -> InvoicesUpdateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a draft sale document. Fields left out keep their value, `lines` replaces every line, and a changed `discountPercent` recomputes the existing lines. Answers 409 when the document is issued or locked, and 422 under the checks of `sales/invoices/create` (the credited document's partner and currency, the OSS and IOSS country, VAT on the lines, the operation type and document series).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**agreement_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[InvoicesUpdateSalesRequestVatScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**deemed_supplier:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvoicesUpdateSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_series_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[InvoicesUpdateSalesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_delete</a>(...) -> InvoicesDeleteSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a draft sale document and release the time entries billed on it. Answers 409 when the document is issued (credit it instead) or locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_issue</a>(...) -> InvoicesIssueSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Issue a draft sale document: assigns the next number (from its document series, else from `series` or the type's default prefix and the year), the issue date (`issueDate`, else the draft's, else today) and a missing due date from the partner's payment term, and for an invoice, credit note or advance invoice posts the journal entry and stores the VAT evidence. `warehouseId` (or the series' warehouse) takes the sold goods of an invoice out of stock with a cost of goods sold entry; `returnToStock` puts them back for a credit note that credits an invoice. A credit note is set against the unpaid balance of the credited document. Emits `sale_invoice.issued`, `sale_invoice.paid` when a credit note settles the credited invoice in full, and `intercompany.invoice_mirrored` when the partner is linked to another company of the group (a draft purchase invoice is created there). Answers 409 when the document is already issued or locked or the accounting period is locked, 422 when the lines carry VAT under a scheme that charges none, when credit notes would exceed the credited total, or when `returnToStock` is used on anything but a credit note of an invoice.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_issue(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**return_to_stock:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_lock</a>(...) -> InvoicesLockSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lock a sale document. A locked document is refused with 409 by `sales/invoices/update`, `sales/invoices/delete`, `sales/invoices/issue` and `sales/invoices/apply-advance` until `sales/invoices/unlock`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_lock(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_unlock</a>(...) -> InvoicesUnlockSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Unlock a sale document locked with `sales/invoices/lock`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_unlock(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_payment_link</a>(...) -> InvoicesPaymentLinkSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the customer payment link of a sale document, rendered from the company's payment link template (`sales/invoices/payment-settings/update`); `url` is null when the company has no template or the document is not issued. The document's payment token is created on first use. Answers 409 when the document is already paid.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_payment_link(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_payment_settings_get</a>() -> InvoicesPaymentSettingsGetSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the company's payment link template, the https URL that `sales/invoices/payment-link`, the invoice PDF and the invoice e-mail fill in for an issued, unpaid document.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_payment_settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_payment_settings_update</a>(...) -> InvoicesPaymentSettingsUpdateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set or clear (null) the company's payment link template: an https URL in which `{{number}}`, `{{amount}}` (the unpaid balance), `{{currency}}`, `{{token}}`, `{{invoiceId}}` and `{{partnerName}}` are replaced, URL-encoded, when a link is rendered.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_payment_settings_update()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**payment_link_template:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_schedules_list</a>(...) -> RecognitionSchedulesListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the revenue recognition schedules: the tranches of deferred income of issued invoices whose lines are recognised ratably, by milestone or by percent complete, each with its status and the journal transaction that recognised it. Filterable by invoiceId, invoiceLineId, status, method and scheduleDate; sortable by scheduleDate and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_schedules_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RecognitionSchedulesListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RecognitionSchedulesListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_apply_advance</a>(...) -> InvoicesApplyAdvanceSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Apply a fully paid advance invoice to an issued invoice of the same partner: posts the settlement journal entry dated `date` (default today), with the applied amount's share of the advance VAT, and records the amount as a payment of the invoice. `amount` defaults to the smaller of the unapplied advance and the invoice's unpaid balance. Emits `sale_invoice.paid` when the invoice becomes fully paid. Answers 409 when the advance is not fully paid, is already applied or credited, when the invoice has nothing left to pay, or when `amount` exceeds the unapplied advance or the unpaid balance; 422 when the advance is not in the company's base currency or the two documents differ in currency.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_apply_advance(
    advance_id="advanceId",
    invoice_id="invoiceId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**advance_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `typing.Optional[str]` — Gross amount of the advance to apply; defaults to the unapplied advance or the unpaid balance of the invoice, whichever is smaller
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoices_list</a>(...) -> InvoicesListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the sale documents of the company with the partner name. Filterable by partnerId, type, status, paymentStatus, fullNumber, issueDate, currency, agreementId, creditedInvoiceId, operationTypeId, documentSeriesId, lockedAt, grossTotal, netTotal, vatTotal, dueDate, orderNumber, seriesLabel, locale and recurringInvoiceId; sortable by createdAt, issueDate, fullNumber, grossTotal, netTotal, vatTotal, status and paymentStatus.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoices_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[InvoicesListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[InvoicesListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_create</a>(...) -> ActsCreateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft delivery act of goods or services (`type`) for a partner, dated `documentDate` (default today). Lines come from `lines`, else from the sale invoice in `saleInvoiceId`, else the act has none; the number is assigned by `sales/acts/issue`. Answers 422 when the sale invoice belongs to another partner or, when its lines are copied, has none.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_create(
    partner_id="partnerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ActsCreateSalesRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transferred_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transferred_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accepted_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accepted_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[ActsCreateSalesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_update</a>(...) -> ActsUpdateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a draft delivery act; fields left out keep their value and `lines` replaces every line. Answers 409 when the act is issued or cancelled, 422 when the linked sale invoice belongs to another partner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ActsUpdateSalesRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transferred_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transferred_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accepted_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accepted_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[ActsUpdateSalesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_issue</a>(...) -> ActsIssueSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Issue a draft delivery act: assigns the next number of its series for the year of the document date. When the act is linked to a sale invoice with pending milestone recognition schedules, they are all recognised on the act's document date, which posts the recognition journal entry and emits `revenue_recognition.posted`. Answers 409 when the act is not a draft, 422 when it has no lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_issue(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_cancel</a>(...) -> ActsCancelSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel a draft or issued delivery act. Answers 409 when it is already cancelled.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_get</a>(...) -> ActsGetSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one delivery act with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_list</a>(...) -> ActsListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List delivery acts. Filterable by status, type, partnerId and documentDate; sortable by createdAt, documentDate and fullNumber.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ActsListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ActsListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">acts_pdf</a>(...) -> ActsPdfSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render a delivery act as a PDF in `locale`, returned base64-encoded, with the number of the linked sale invoice when there is one.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.acts_pdf(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[ActsPdfSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoice_templates_create</a>(...) -> InvoiceTemplatesCreateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a named template for invoices or credit notes (`documentType`): the header defaults and the lines that `sales/recurring-invoices/generate` turns into invoices. Answers 422 when a referenced partner, agreement, operation type, document series, catalog item or project does not exist or the series is for another document type; 409 when a template with that name exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoice_templates_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `typing.Optional[InvoiceTemplatesCreateSalesRequestDocumentType]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_term_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[InvoiceTemplatesCreateSalesRequestVatScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**agreement_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_series_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supply_type:** `typing.Optional[InvoiceTemplatesCreateSalesRequestSupplyType]` 
    
</dd>
</dl>

<dl>
<dd>

**series_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[InvoiceTemplatesCreateSalesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoice_templates_update</a>(...) -> InvoiceTemplatesUpdateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a template; fields left out keep their value and `lines` replaces every line. The 422 reference checks of `sales/invoice-templates/create` apply; 409 when the new name is taken.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoice_templates_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `typing.Optional[InvoiceTemplatesUpdateSalesRequestDocumentType]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_term_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[InvoiceTemplatesUpdateSalesRequestVatScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**agreement_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_series_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**discount_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**received_by_title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**supply_type:** `typing.Optional[InvoiceTemplatesUpdateSalesRequestSupplyType]` 
    
</dd>
</dl>

<dl>
<dd>

**series_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[InvoiceTemplatesUpdateSalesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoice_templates_get</a>(...) -> InvoiceTemplatesGetSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one invoice template.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoice_templates_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoice_templates_delete</a>(...) -> InvoiceTemplatesDeleteSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete an invoice template.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoice_templates_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">invoice_templates_list</a>(...) -> InvoiceTemplatesListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List invoice templates. Filterable by name, documentType and partnerId; sortable by name, documentType and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.invoice_templates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[InvoiceTemplatesListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[InvoiceTemplatesListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_create</a>(...) -> RecurringInvoicesCreateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a schedule that generates invoices from an invoice template every `interval` periods of `frequency` from `startDate` (the first run) until `endDate`, for `partnerId` or else the template's partner. `autoIssue` issues each generated invoice and `autoSend` e-mails it to `sendTo`, else to the partner. Invoices are generated by `sales/recurring-invoices/run`, `sales/recurring-invoices/generate` and the scheduled job `recurring-invoices`. Answers 422 when the template is a credit note template, when neither the schedule nor the template names a partner, when `endDate` is before `startDate`, or when `autoSend` is set without `autoIssue`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_create(
    template_id="templateId",
    start_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**template_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**start_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**frequency:** `typing.Optional[RecurringInvoicesCreateSalesRequestFrequency]` 
    
</dd>
</dl>

<dl>
<dd>

**interval:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[RecurringInvoicesCreateSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_issue:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_send:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**send_to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_update</a>(...) -> RecurringInvoicesUpdateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a schedule; fields left out keep their value. A change of `startDate`, `frequency` or `interval` moves `nextRunDate` to the first occurrence of the new grid on or after the current next run (or the new start date, if later); an explicit `nextRunDate` wins. `status` switches between `active` and `paused`; a next run past `endDate` makes the schedule `finished`. The 422 checks of `sales/recurring-invoices/create` apply.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**template_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**frequency:** `typing.Optional[RecurringInvoicesUpdateSalesRequestFrequency]` 
    
</dd>
</dl>

<dl>
<dd>

**interval:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**start_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**next_run_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[RecurringInvoicesUpdateSalesRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[RecurringInvoicesUpdateSalesRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_issue:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_send:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**send_to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_get</a>(...) -> RecurringInvoicesGetSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one recurring invoice schedule with the names of its template and partner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_delete</a>(...) -> RecurringInvoicesDeleteSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a recurring invoice schedule. The invoices it generated stay.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_generate</a>(...) -> RecurringInvoicesGenerateSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate the next invoice of a schedule now, dated its `nextRunDate`: creates a draft from the template (due date from the template's payment term, VAT scheme from the template or else resolved for the partner and supply type), issues it when `autoIssue` is set and e-mails it when `autoSend` is set, then moves the schedule to its next occurrence (or to `finished` after the last one) and emits `recurring_invoice.generated`. A failure to issue or send comes back in `error` and is stored as `lastError`; the draft stays. Answers 409 when the schedule is finished, 422 when the template is a credit note template or has no lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_generate(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_run</a>(...) -> RecurringInvoicesRunSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate every invoice due up to `asOfDate` (default today) from the active schedules of the company, catching up to 60 missed occurrences per schedule, as `sales/recurring-invoices/generate` does for one; each generated invoice emits `recurring_invoice.generated`. The answer lists what was generated and the schedules that failed; a failure is also stored as the schedule's `lastError`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_run()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recurring_invoices_list</a>(...) -> RecurringInvoicesListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List recurring invoice schedules with the names of their template and partner. Filterable by status, partnerId, templateId, frequency, nextRunDate and autoIssue; sortable by nextRunDate, startDate, status, frequency and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recurring_invoices_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RecurringInvoicesListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RecurringInvoicesListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_compute</a>(...) -> RecognitionComputeSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Preview the pending ratable revenue schedules due on or before `asOfDate` (default the company's current date) with their total; nothing is posted. `sales/recognition/run` posts them.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_compute()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_run</a>(...) -> RecognitionRunSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Recognise deferred revenue: posts one journal entry dated `postingDate` (default `asOfDate`, default the company's current date) that debits the deferred income account and credits each line's revenue account, for the pending ratable schedules due on or before `asOfDate` or for exactly the `scheduleIds` given, marks them recognised, records a run with trigger `manual` and emits `revenue_recognition.posted`. Answers 422 when nothing is due or a given schedule is missing or no longer pending, and 409 when the posting period is locked. Due ratable schedules are also posted by the scheduler once their date has passed (trigger `schedule_due`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_run()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**posting_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**schedule_ids:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_progress</a>(...) -> RecognitionProgressSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Report the percentage of completion of a `percent_complete` invoice line and recognise the revenue up to it: a schedule for the difference between the revenue due at that percentage and the amount already recognised is created and posted at once, dated `date` (default the company's current date), as a run with trigger `progress` that emits `revenue_recognition.posted`. Refused with 422 when the line is not `percent_complete`, the invoice is not an issued standard invoice, the percentage is 0 or above 100, or nothing new is to be recognised; 409 when the period is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_progress(
    invoice_line_id="invoiceLineId",
    percent_complete="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**invoice_line_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**percent_complete:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_modify</a>(...) -> RecognitionModifySalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Apply an IFRS 15 contract modification to a deferred invoice line. Prospective: cancel the pending schedule and respread the unrecognized remainder over the new terms. Cumulative catch-up (ratable only): recompute revenue as if the new terms applied from the start and post the difference immediately.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_modify(
    invoice_line_id="invoiceLineId",
    approach="prospective",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**invoice_line_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**approach:** `RecognitionModifySalesRequestApproach` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**new_end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**new_milestones:** `typing.Optional[typing.List[RecognitionModifySalesRequestNewMilestonesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_runs_list</a>(...) -> RecognitionRunsListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the revenue recognition runs, newest first; filterable by `runDate` and `trigger`, sortable by `runDate` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_runs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RecognitionRunsListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RecognitionRunsListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_summary</a>(...) -> RecognitionSummarySalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deferred revenue per line of the issued standard invoices whose recognition method is not `point_in_time`: the deferred total, the amount recognised so far, the remainder, the number of pending schedules and the next schedule date, with totals; `invoiceId` limits it to one invoice. For a `percent_complete` line the deferred total is the line's base amount, for the other methods the sum of its schedules.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.recognition_summary()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">refund_liability_list</a>(...) -> RefundLiabilityListSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the refund liabilities of issued invoices (created at issue from the lines' `refundEstimatePercent` or by `sales/refund-liability/true-up`): the estimate, the part consumed by credit notes, the settlement refunds and the remaining amount (estimate less consumed), with the invoice number. Filterable by invoiceId; sortable by createdAt and updatedAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.refund_liability_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RefundLiabilityListSalesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RefundLiabilityListSalesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">refund_liability_true_up</a>(...) -> RefundLiabilityTrueUpSalesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Re-estimate the refund liability of an issued standard invoice to `estimatedTotal` and post the difference on `date` (default today) between the refund liability account and the invoice's revenue accounts, in proportion to the lines' allocated or net amounts; creates the liability when the invoice has none. Emits `refund_liability.trued_up`. Answers 422 when the invoice is not an issued standard invoice, when the estimate is below the amount already consumed or unchanged, or when the invoice has no revenue to allocate against; 409 when the accounting period is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.refund_liability_true_up(
    invoice_id="invoiceId",
    estimated_total="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**invoice_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**estimated_total:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## OperationTypes
<details><summary><code>client.operation_types.<a href="src/nordlet/operation_types/client.py">create</a>(...) -> CreateOperationTypesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an operation type: a `code` with the flags that say what it is for (`isSale`, `isPurchase`, ...), an optional `invoiceType` (`invoice`, `credit_note`, `proforma`, `advance`) and optional account codes. An invoice names it in `operationTypeId`: a sale invoice needs `isSale` and a matching `invoiceType`, a purchase invoice `isPurchase`, and the type's account codes then replace the default posting accounts when the invoice is issued (`sales/invoices/issue`) or registered (`purchases/invoices/register`). `includeInVatRegister: false` keeps the type's invoices out of the Lithuanian i.SAF and FR0600, `includeInSaft: false` out of the SAF-T file. Account codes must exist and be postable and `payerPartnerId` must be an active partner (422 otherwise); a repeated `code` is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.operation_types.create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_type:** `typing.Optional[CreateOperationTypesRequestInvoiceType]` 
    
</dd>
</dl>

<dl>
<dd>

**payer_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**debit_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**credit_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**advance_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**income_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_purchase:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_sale:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_write_off:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_internal_movement:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_purchase_return:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_sales_return:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_consignment:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_production:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_asset_in:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_asset_out:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_cash_register_sale:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**include_in_vat_register:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**include_in_saft:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.operation_types.<a href="src/nordlet/operation_types/client.py">update</a>(...) -> UpdateOperationTypesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change an operation type's fields; omitted ones keep their value. A `code` already used by another type is refused with 409, a body without changes with 400.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.operation_types.update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_type:** `typing.Optional[UpdateOperationTypesRequestInvoiceType]` 
    
</dd>
</dl>

<dl>
<dd>

**payer_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**debit_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**credit_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**advance_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**income_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_purchase:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_sale:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_write_off:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_internal_movement:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_purchase_return:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_sales_return:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_consignment:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_production:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_asset_in:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_asset_out:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_cash_register_sale:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**include_in_vat_register:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**include_in_saft:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**sort_order:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.operation_types.<a href="src/nordlet/operation_types/client.py">get</a>(...) -> GetOperationTypesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one operation type.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.operation_types.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.operation_types.<a href="src/nordlet/operation_types/client.py">delete</a>(...) -> DeleteOperationTypesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete an operation type that no sale invoice, purchase invoice or document series refers to. Otherwise the call is refused with 409; deactivate the type with `operation-types/update` instead.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.operation_types.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.operation_types.<a href="src/nordlet/operation_types/client.py">list</a>(...) -> ListOperationTypesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List operation types. Filterable by `code`, `name`, `isSale`, `isPurchase` and `isActive`; sortable by `code`, `name`, `sortOrder` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.operation_types.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListOperationTypesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListOperationTypesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## DocumentSeries
<details><summary><code>client.document_series.<a href="src/nordlet/document_series/client.py">create</a>(...) -> CreateDocumentSeriesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a numbering series for sale invoices, credit notes, proformas or advance invoices (`documentType`). Numbers run from `nextNumber`, padded to `numberLength` digits, and are written as `prefix`-number or, with `printSeries` false, as the bare number; a series may be bound to an operation type (a default series of an operation type is picked for its documents that name no series) and to a warehouse, which `sales/invoices/issue` takes the goods from. `isDefault` makes it the default of its document type and clears the previous one. Answers 422 when only one end of the allocated range `allocatedFrom`..`allocatedTo` is given or the range is reversed, 409 when the prefix exists for the document type.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.document_series.create(
    prefix="prefix",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**prefix:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `typing.Optional[CreateDocumentSeriesRequestDocumentType]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**number_length:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**next_number:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**allocated_from:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**allocated_to:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**print_series:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.document_series.<a href="src/nordlet/document_series/client.py">update</a>(...) -> UpdateDocumentSeriesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a document series; fields left out keep their value. `nextNumber` cannot go below its current value (409); `isDefault` clears the previous default of the document type. Answers 422 for an incomplete or reversed allocated range, 409 when the prefix is taken for the document type.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.document_series.update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `typing.Optional[UpdateDocumentSeriesRequestDocumentType]` 
    
</dd>
</dl>

<dl>
<dd>

**prefix:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**number_length:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**next_number:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**allocated_from:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**allocated_to:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**print_series:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.document_series.<a href="src/nordlet/document_series/client.py">get</a>(...) -> GetDocumentSeriesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one document series.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.document_series.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.document_series.<a href="src/nordlet/document_series/client.py">delete</a>(...) -> DeleteDocumentSeriesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a document series no sale document uses. Answers 409 when invoices reference it; deactivate it with `isActive` instead.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.document_series.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.document_series.<a href="src/nordlet/document_series/client.py">list</a>(...) -> ListDocumentSeriesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List document series. Filterable by documentType, prefix, operationTypeId and isActive; sortable by prefix, documentType and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.document_series.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListDocumentSeriesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListDocumentSeriesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## purchases
<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_create</a>(...) -> InvoicesCreatePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft purchase invoice or credit note (`type`) from a supplier document; it is posted with `purchases/invoices/register`. Lines without a unit price take the item's supplier or purchase price, `currency` defaults to the company's invoice currency, `documentRef` links an uploaded file, and the gross total leaves out self-assessed VAT. `creditedInvoiceId` (credit notes only) must be an invoice of the same partner, `purchaseOrderId` an order of the same partner that is not draft, submitted or cancelled, and `operationTypeId` an active purchase operation type, each 422 otherwise; the same `documentNumber` for the same partner is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.purchases import InvoicesCreatePurchasesRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_create(
    partner_id="partnerId",
    document_number="documentNumber",
    document_date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        InvoicesCreatePurchasesRequestLinesItem()
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[InvoicesCreatePurchasesRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[InvoicesCreatePurchasesRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**credited_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_order_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**einvoice_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_get</a>(...) -> InvoicesGetPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one purchase invoice or credit note with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_update</a>(...) -> InvoicesUpdatePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a draft purchase invoice (409 once registered); only the fields sent are changed, and `lines` replace all existing lines with the totals recomputed. `purchaseOrderId` and `operationTypeId` are checked as on `purchases/invoices/create` (422). A `documentNumber` already used for the partner is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_order_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_transport_mode:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_region:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**intrastat_nature_of_transaction:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**einvoice_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[InvoicesUpdatePurchasesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_delete</a>(...) -> InvoicesDeletePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark a draft purchase invoice as deleted (409 once registered). A document capture linked to it goes back to `extracted` (or `pending` when it has no extraction) and can be confirmed again.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_register</a>(...) -> InvoicesRegisterPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a draft purchase invoice or credit note: posts the journal entry dated `registrationDate` (default the document date) and sets the status to `registered`. The entry debits each line's expense account (the line's `accountCode`, else the item's purchase or expense account, else the operation type's expense account, else the `purchases.goodsForResale` or `purchases.defaultExpense` rule account), debits VAT receivable (a company that is not a VAT payer books the VAT into the expense instead), credits payables (the operation type's credit account when set) and credits output VAT for self-assessed VAT; a credit note posts the reverse. Lines with `deferralStartDate` and `deferralEndDate` are debited to the `purchases.prepaidExpenses` account instead and get a monthly release schedule for `purchases/deferrals/post`. With `warehouseId` the product lines of an invoice are received into stock at their base-currency cost (422 on an order-linked invoice, whose goods arrive through `purchases/receipts/create`, and for a line that is also deferred); `returnFromStock` on a credit note that credits an invoice takes the goods back out of stock at their FIFO cost and books the difference to the credited amount on the `inventory.cogs` account (422 on an invoice, without `creditedInvoiceId`, or when no goods of the credited invoice are in stock). A credit note that credits a registered invoice in the same currency is applied to it as a payment up to the open amount. Refused with 409 when already registered or the accounting period is locked, and with 422 when the credit notes would exceed the credited invoice, a posting account is missing or no exchange rate exists for the date. Emits `purchase_invoice.registered`, `purchase_invoice.paid` when the credited invoice becomes fully paid, and `stock.changed` when stock moves.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_register(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**registration_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**return_from_stock:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">deferrals_list</a>(...) -> DeferralsListPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the monthly release rows that `purchases/invoices/register` creates for lines booked as prepaid expenses, each with its amount, expense and prepaid account and `status` (`pending`, `posted`, `cancelled`). Filterable by `invoiceId`, `status` and `scheduleDate`; sortable by `scheduleDate`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.deferrals_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DeferralsListPurchasesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DeferralsListPurchasesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">deferrals_post</a>(...) -> DeferralsPostPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Post every `pending` prepaid-expense release row dated on or before `asOfDate` (default today in the company's time zone): one journal entry per schedule date debiting the expense account and crediting the prepaid account, and the rows become `posted`. A locked accounting period is refused with 409. The scheduled job `expense-deferrals` runs the same release for every active company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.deferrals_post()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_list</a>(...) -> InvoicesListPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List purchase invoices and credit notes without lines, with the supplier's `partnerName`. Filterable by `partnerId`, `type`, `status`, `paymentStatus`, `documentNumber`, `documentDate`, `currency`, `operationTypeId`, `purchaseOrderId`, `grossTotal`, `netTotal`, `vatTotal` and `dueDate`; sortable by `createdAt`, `documentDate`, `documentNumber`, `grossTotal` and `dueDate`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[InvoicesListPurchasesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[InvoicesListPurchasesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_create</a>(...) -> OrdersCreatePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft purchase order for a supplier. Lines without a unit price take the item's supplier or purchase price; `orderNumber` comes from the `purchase_order` series with prefix PO when not given; `currency` defaults to the company's invoice currency; `documentRef` links an uploaded file to the order. A number already in use is refused with 409. The order continues with `purchases/orders/submit`, `purchases/orders/approve` and `purchases/receipts/create`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.purchases import OrdersCreatePurchasesRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_create(
    partner_id="partnerId",
    order_date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        OrdersCreatePurchasesRequestLinesItem()
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**order_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[OrdersCreatePurchasesRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expected_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_update</a>(...) -> OrdersUpdatePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a draft purchase order (409 once it is submitted); only the fields sent are changed. `lines` replace all existing lines and the totals are recomputed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**expected_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[OrdersUpdatePurchasesRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_get</a>(...) -> OrdersGetPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one purchase order with its lines; each line carries `receivedQty` and `remainingQty`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_list</a>(...) -> OrdersListPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List purchase orders without lines, with the supplier's `partnerName`. Filterable by `partnerId`, `status`, `orderNumber`, `orderDate`, `currency` and `grossTotal`; sortable by `createdAt`, `orderDate`, `orderNumber` and `grossTotal`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[OrdersListPurchasesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[OrdersListPurchasesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_submit</a>(...) -> OrdersSubmitPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Move a `draft` purchase order to `submitted` for approval (409 from any other status). `reason` is kept in the audit log.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_submit(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_approve</a>(...) -> OrdersApprovePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Approve a `submitted` purchase order (409 from any other status), recording who approved it and when; needs the `purchases:approve` scope. Goods are then received with `purchases/receipts/create`. Emits `purchase_order.approved`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_approve(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_reject</a>(...) -> OrdersRejectPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send a `submitted` purchase order back to `draft` (409 from any other status); needs the `purchases:approve` scope. `reason` is kept in the audit log.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_reject(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_cancel</a>(...) -> OrdersCancelPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel a `draft`, `submitted` or `approved` purchase order (409 from any other status, or when the order already has a goods receipt).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_close</a>(...) -> OrdersClosePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Close an `approved`, `partially_received` or `received` purchase order (409 from any other status); a closed order accepts no further goods receipts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_close(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">orders_delete</a>(...) -> OrdersDeletePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark a `draft` purchase order as deleted (409 once it is submitted).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.orders_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">receipts_create</a>(...) -> ReceiptsCreatePurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a goods receipt against an `approved` or `partially_received` purchase order (409 otherwise), numbered from the `goods_receipt` series with prefix GR. Lines whose item is a product go into stock in `warehouseId`, else the order's warehouse (422 when neither is set), at their share of the order line's net amount converted at the receipt date's rate; `lotNumber` and `expiryDate` receive them into a lot, and an item that needs lot or serial tracking is refused with 422 without one. A quantity above the line's remaining quantity is refused with 409; the order becomes `received` when every line is fully received, else `partially_received`. Emits `goods_receipt.posted`, `stock.changed` and, when fully received, `purchase_order.received`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.purchases import ReceiptsCreatePurchasesRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.receipts_create(
    order_id="orderId",
    receipt_date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        ReceiptsCreatePurchasesRequestLinesItem(
            order_line_id="orderLineId",
            quantity="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**order_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**receipt_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[ReceiptsCreatePurchasesRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">receipts_get</a>(...) -> ReceiptsGetPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one goods receipt with its lines and their stock movement ids.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.receipts_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">receipts_list</a>(...) -> ReceiptsListPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List goods receipts without lines. Filterable by `orderId`, `warehouseId`, `receiptDate` and `receiptNumber`; sortable by `createdAt` and `receiptDate`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.receipts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ReceiptsListPurchasesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ReceiptsListPurchasesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">invoices_match</a>(...) -> InvoicesMatchPurchasesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compare a purchase invoice with its linked purchase order and the goods received so far, grouped by item (by description for lines without one). Each row is `matched`, `not_received` (invoiced but nothing received), `over_invoiced` (invoiced more than received), `price_mismatch` (unit price differs by more than `priceTolerancePercent`), `not_on_order` or `not_invoiced`; `status` is `mismatched` when any row other than `not_invoiced` is not matched. Refused with 422 when the invoice has no `purchaseOrderId` or its currency differs from the order's. Nothing is changed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.invoices_match(
    invoice_id="invoiceId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**invoice_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**price_tolerance_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## capture
<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">settings_get</a>() -> SettingsGetCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the company's document capture settings: whether intake by e-mail is enabled, whether e-mailed documents are read on arrival, the company's intake e-mail address and whether a reading provider is configured. The intake token behind the address is created on the first call.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">settings_update</a>(...) -> SettingsUpdateCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Switch `intakeEnabled` (documents sent to the intake address are accepted) and `captureAutoExtract` (they are read on arrival) on or off; at least one field is required.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.settings_update()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**intake_enabled:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**capture_auto_extract:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">settings_regenerate_intake</a>() -> SettingsRegenerateIntakeCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replace the company's intake token, so the previous intake e-mail address stops working and the settings come back with the new one.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.settings_regenerate_intake()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">inbound_email</a>(...) -> InboundEmailCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Endpoint for the inbound e-mail provider (Postmark field names or the generic `to`, `from`, `subject` and `attachments` form). It needs the `x-inbound-secret` header and finds the company by the `intake+<token>@` recipient address (404 when unknown, 403 when intake is disabled). Every PDF, image, Word or PowerPoint attachment up to 10 MB becomes a `pending` capture (`accepted`), anything else is `skipped`; when the company has automatic reading on, is not on trial and a reading provider is configured, each capture is read at once.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.inbound_email()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**postmark_to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**to_full:** `typing.Optional[typing.List[InboundEmailCaptureRequestToFullItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**postmark_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**postmark_subject:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**postmark_attachments:** `typing.Optional[typing.List[InboundEmailCaptureRequestAttachmentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `typing.Optional[InboundEmailCaptureRequestTo]` 
    
</dd>
</dl>

<dl>
<dd>

**from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**subject:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attachments:** `typing.Optional[typing.List[InboundEmailCaptureRequestAttachmentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_upload</a>(...) -> DocumentsUploadCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Upload a supplier document (PDF, image, Word or PowerPoint, up to 10 MB; 422 for any other type) as a capture and read it at once. The result holds the extracted supplier, dates, totals and lines, the partner matched by VAT code, then partner code, then name, the raw text, and `status` `extracted` or `failed` with `error`. Needs a configured reading provider, is refused with 402 for a company on trial until its first top-up, and counts every page read as `ocr_page` usage. The draft is reviewed and saved with `capture/documents/confirm`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_upload(
    file_name="fileName",
    mime_type="mimeType",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**file_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**mime_type:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` — Base64-encoded scan, photo or PDF of the supplier document
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_extract</a>(...) -> DocumentsExtractCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read a stored capture again and replace its draft (supplier, totals, lines, matched partner). A capture received over Peppol is parsed from its document again without a reading provider; any other needs the provider and, for a company on trial, the first top-up (402). Refused with 409 once the capture is linked to a purchase invoice.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_extract(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_get</a>(...) -> DocumentsGetCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one capture with its extraction and raw text.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_list</a>(...) -> DocumentsListCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List captures without raw text. Filterable by `status`, `matchedPartnerId` and `purchaseInvoiceId`; sortable by `createdAt` and `updatedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DocumentsListCaptureRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DocumentsListCaptureRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_delete</a>(...) -> DocumentsDeleteCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a capture and its stored file (409 once it is linked to a purchase invoice).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">documents_confirm</a>(...) -> DocumentsConfirmCaptureResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates the purchase invoice (or credit note, see `type`) from `lines`. Lines with the opposite sign go in `oppositeLines` and are saved as a second document of the opposite type for the same supplier: a purchase credit note against the new invoice, or a purchase invoice next to the new credit note. It is numbered `oppositeDocumentNumber`, by default the document number followed by "-CR" (credit note) or "-INV" (invoice).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.capture import DocumentsConfirmCaptureRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.documents_confirm(
    id="id",
    document_number="documentNumber",
    document_date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        DocumentsConfirmCaptureRequestLinesItem()
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[DocumentsConfirmCaptureRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**new_supplier:** `typing.Optional[DocumentsConfirmCaptureRequestNewSupplier]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[DocumentsConfirmCaptureRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**opposite_lines:** `typing.Optional[typing.List[DocumentsConfirmCaptureRequestOppositeLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**opposite_document_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## peppol
<details><summary><code>client.peppol.<a href="src/nordlet/peppol/client.py">participants_lookup</a>(...) -> ParticipantsLookupPeppolResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Look a receiver up on the Peppol network (SML and SMP) and say which Peppol BIS Billing 3.0 documents it accepts. Give `partnerId` to look up a partner by its Peppol ID, VAT code or registration code, or `participantId` as "<scheme>:<identifier>". Works without an access point.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.peppol.participants_lookup()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**participant_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.peppol.<a href="src/nordlet/peppol/client.py">webhooks</a>(...) -> WebhooksPeppolResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Apply one event: a delivery status event updates the Peppol status of the sale invoice with that message id and, when the status changes, emits `sale_invoice.peppol_delivered`, `sale_invoice.peppol_rejected` or `sale_invoice.peppol_failed`; a received-document event fetches the document from the access point, stores it as a document capture with the matched supplier, emits `document_capture.peppol_received` and marks it read at the access point (a document already stored is skipped). `handled` is false when the event matched no invoice or document. Answers 404 when no company uses that provider account, 401 when the signature does not match.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.peppol.webhooks(
    provider="recommand",
    company_id="companyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**provider:** `WebhooksPeppolRequestProvider` 
    
</dd>
</dl>

<dl>
<dd>

**company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## declarations
<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_intrastat_compute</a>(...) -> LtIntrastatComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the Lithuanian Intrastat report of a month for one flow as the IDAIS INTRASTATReportSubmission XML: dispatches from the issued sale invoices and purchase credit notes, arrivals from the registered purchase invoices and sale credit notes, grouped into report items. `transactionNature`, `deliveryTerms`, `transportMode` and `regionCode` are the defaults for lines without their own values; `statisticalValueRequired` adds the statistical value to each item. Answers 422 when the company is not a VAT payer. With `persist`, the file is stored and a submission for `lt-intrastat-arrivals` or `lt-intrastat-dispatches` is created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_intrastat_compute(
    year=1000000,
    month=1000000,
    flow="arrivals",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**flow:** `LtIntrastatComputeDeclarationsRequestFlow` 
    
</dd>
</dl>

<dl>
<dd>

**transaction_nature:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**delivery_terms:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transport_mode:** `typing.Optional[LtIntrastatComputeDeclarationsRequestTransportMode]` 
    
</dd>
</dl>

<dl>
<dd>

**region_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**statistical_value_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**preparation_time_hours:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**preparation_time_minutes:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**persist:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_ivaz_generate</a>(...) -> LtIvazGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the i.VAZ transport document message (iVAZ1.3.3) for up to 100 issued waybills and returns the XML. Answers 422 when the registration code of the company is not numeric or when a waybill is not issued. With `persist`, the file is stored and a submission for `lt-ivaz` is created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_ivaz_generate(
    waybill_ids=[
        "waybillIds"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**waybill_ids:** `typing.List[str]` 
    
</dd>
</dl>

<dl>
<dd>

**persist:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_intrastat_obligation</a>(...) -> LtIntrastatObligationDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Checks the Intrastat reporting obligation of a year per flow: the value of goods traded with other Member States in the previous year, the month from which reporting is due (January when that value already passed the reporting threshold, else the month the cumulative value of the year passes it), whether the statistical value is required, and the monthly values. Answers 422 when no thresholds are stored for the year.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_intrastat_obligation(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_isaf_generate</a>(...) -> LtIsafGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the Lithuanian i.SAF register XML of a month: `dataType` F covers both registers, S the issued sale invoices only, P the registered purchase invoices only. Returns the XML without storing it; `declarations/submissions/create` stores it as a submission.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_isaf_generate(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**data_type:** `typing.Optional[LtIsafGenerateDeclarationsRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_fr0600compute</a>(...) -> LtFr0600ComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the fields of the Lithuanian VAT return FR0600 for the period of `months` months starting in `month`, with the breakdown by VAT classifier behind them. `deductionPercent` is the share of input VAT deducted and is written to field 28.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_fr0600compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**deduction_percent:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_gpm313compute</a>(...) -> LtGpm313ComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes fields 5 to 7 of the monthly GPM313 from the payroll run of the month the pay was earned: the run of the previous month with `payoutTiming` `next-month`, the run of the same month with `same-month`. `paymentDay` decides whether the withheld tax goes to field 6 (paid by the 15th) or field 7 (after it). Fields 8 to 12 are returned as zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_gpm313compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**payout_timing:** `typing.Optional[LtGpm313ComputeDeclarationsRequestPayoutTiming]` 
    
</dd>
</dl>

<dl>
<dd>

**payment_day:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_sam_compute</a>(...) -> LtSamComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the monthly SAM figures from the payroll run of the month: per employee the insured income, the employee and employer contributions together and the resulting tariff, plus the insured count and the totals. A missing run or a run still in draft is reported in the warnings.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_sam_compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_sd_generate</a>(...) -> LtSdGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the rows of the 1-SD (employment contracts that start in the date range) or of the 2-SD (contracts that ended in the range, with the final insured income and contributions from the payroll line of the termination month). Answers 422 when `fromDate` is after `toDate`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_sd_generate(
    type="1-SD",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `LtSdGenerateDeclarationsRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_saft_generate</a>(...) -> LtSaftGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the Lithuanian SAF-T (version 2.01) XML for a date range: `dataType` F is the full file, GL, SI, PI, PA, MG and AS limit it to the general ledger, sale invoices, purchase invoices, payments, movements of goods or asset transactions. Answers 422 when `fromDate` is after `toDate`. With `persist`, the file is stored and a submission for `lt-saft` is created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_saft_generate(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**data_type:** `typing.Optional[LtSaftGenerateDeclarationsRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**persist:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_ivaz_amend</a>(...) -> LtIvazAmendDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds an i.VAZ amendment message for up to 100 issued waybills, carrying their current data as TransportDocumentAmendment elements. Answers 422 when the registration code of the company is not numeric or when a waybill is not issued. With `persist`, the file is stored and a submission for `lt-ivaz-amendment` is created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_ivaz_amend(
    waybill_ids=[
        "waybillIds"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**waybill_ids:** `typing.List[str]` 
    
</dd>
</dl>

<dl>
<dd>

**persist:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_ivaz_cancel</a>(...) -> LtIvazCancelDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds an i.VAZ cancellation message for up to 100 waybills, each with a cancellation reason code and optional additional information. Answers 422 when the registration code of the company is not numeric; a waybill that was never issued is reported in the warnings. With `persist`, the file is stored and a submission for `lt-ivaz-cancellation` is created.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.declarations import LtIvazCancelDeclarationsRequestEntriesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_ivaz_cancel(
    entries=[
        LtIvazCancelDeclarationsRequestEntriesItem(
            waybill_id="waybillId",
            reason="1",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**entries:** `typing.List[LtIvazCancelDeclarationsRequestEntriesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**persist:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_fr0564compute</a>(...) -> LtFr0564ComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the rows of the Lithuanian FR0564 report of a month from the issued sale invoices and credit notes with the `intra_eu_b2b` or `reverse_charge` scheme: one row per buyer VAT number of another Member State, with goods and services split by the type of the catalogue item. Invoices not in EUR and buyers without a valid EU VAT number are left out and named in the warnings; the triangular column is always zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_fr0564compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_gpm312compute</a>(...) -> LtGpm312ComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the rows of the annual GPM312 from the payroll runs of the payout months of the year (December of the previous year to November with `payoutTiming` `next-month`, January to December with `same-month`): one row per employee and payment type code, with the amount paid, the tax withheld and the rate applied.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_gpm312compute(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**payout_timing:** `typing.Optional[LtGpm312ComputeDeclarationsRequestPayoutTiming]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_pln204compute</a>(...) -> LtPln204ComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the boxes of the Lithuanian annual corporate income tax return PLN204 for the fiscal year from the financial statements and the tax adjustments recorded with `declarations/tax-adjustments/create`: the PLN204S annex from the `non_deductible` adjustments and the PLN204Z annex from the `non_taxable_income` ones, by their `code`. The small-entity rate is applied when the size criteria allow it. Answers 422 when such an adjustment has no code or a code the annex does not list, or when no rate table covers the period.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_pln204compute(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_oss_compute</a>(...) -> EuOssComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the Union OSS return of a quarter from the issued invoices and credit notes with the `oss_union` VAT scheme: one row per Member State of consumption and VAT rate, classified as standard or reduced, and a corrections section for the credit notes that credit invoices of earlier periods. Amounts are in EUR, converted at the official rate of the last day of the period. Answers 422 when the company is not established in the EU.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_oss_compute(
    year=1000000,
    quarter=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**quarter:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_ioss_compute</a>(...) -> EuIossComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the IOSS return of a month from the issued invoices and credit notes with the `ioss` VAT scheme, with the same rows, corrections and EUR conversion as `declarations/eu/oss/compute`. Answers 422 when the company is not established in the EU.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_ioss_compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_own_goods_transfers_compute</a>(...) -> EuOwnGoodsTransfersComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the monthly return of the special scheme for transfers of own goods from the warehouse transfers between warehouses in two different EU Member States: one row per destination and dispatch country with the cost of the goods as the taxable amount in EUR, the transfers behind the rows, and the due date. Answers 422 when the company is not established in the EU.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_own_goods_transfers_compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_digital_reporting_list</a>(...) -> EuDigitalReportingListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the transactions of a date range that fall under EU digital reporting: issued sale invoices and credit notes with the `intra_eu_b2b` or `reverse_charge` scheme to EU customers, and registered purchase invoices from suppliers in other Member States whose lines carry a self-assessed VAT classifier. Each transaction names the article it is reported under, the Member State it is reported to, its deadline and the data still missing. Answers 422 when the company is not identified for VAT in the EU.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_digital_reporting_list(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_dac7preview</a>(...) -> EuDac7PreviewDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Which platform sellers are reportable for the year (Council Directive (EU) 2021/514, Annex V) and why the others are excluded, the data still missing, and how the company files the report in its Member State.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_dac7preview(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_dac7xml</a>(...) -> EuDac7XmlDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the DAC7 (DPI) XML report of a year for the Member State of the company and returns it base64-encoded with the file name the administration expects. Answers 422 when no DAC7 filing channel exists for the company country. The sellers and the missing data behind it come from `declarations/eu/dac7/preview`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_dac7xml(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_distance_sales_threshold_get</a>(...) -> EuDistanceSalesThresholdGetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Sums the cross-border sales to EU consumers (invoices under the `oss_union` scheme, and domestic-scheme invoices to partners without a VAT number in another Member State) of the current and the preceding calendar year as of `date` (default: the current date of the company) and compares both with the EUR 10 000 distance sales threshold.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_distance_sales_threshold_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_union_turnover_get</a>(...) -> EuUnionTurnoverGetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Sums the turnover of the company within the Union (issued invoices and credit notes other than export and out-of-scope supplies) for the current and the previous calendar year as of `date` (default: the current date of the company) and compares it with the EUR 100 000 cap of the cross-border SME scheme. The status is `not_applicable` for a registered VAT payer, otherwise `below`, `approaching` or `exceeded`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_union_turnover_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_sme_cross_border_report_compute</a>(...) -> EuSmeCrossBorderReportComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the quarterly report of the cross-border SME scheme: the value of the issued supplies within the Union per Member State of supply (the VAT country of the invoice, else the country of the partner, else the home country), in the base currency of the company. Supplies that resolve to a non-EU country are left out and named in the warnings.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_sme_cross_border_report_compute(
    year=1000000,
    quarter=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**quarter:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_sme_thresholds_list</a>() -> EuSmeThresholdsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the stored table of national SME VAT exemption thresholds per Member State, with sector thresholds and intra-EU acquisition triggers where recorded, and the national and Union-wide caps of the directive. No company data is read.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_sme_thresholds_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_sme_threshold_get</a>(...) -> EuSmeThresholdGetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compares the gross turnover of the company in the current calendar year as of `date` (default: the current date of the company) with the national SME exemption threshold of its country. The status is `not_applicable` for a registered VAT payer, `unknown` when no threshold is on file or its currency differs from the base currency, otherwise `below`, `approaching` or `exceeded`; when the country has an intra-EU acquisitions trigger, the acquisitions from and services to other Member States are compared with it too.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_sme_threshold_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_vat_return_packs_list</a>() -> EuVatReturnPacksListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the national VAT return forms Nordlet can compute, with the country, form key, form name, filing frequency and source.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_vat_return_packs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">eu_vat_return_compute</a>(...) -> EuVatReturnComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Computes the national VAT return of `countryCode` for the period of `months` months starting in `month`, as the numbered boxes of the form with labels and amounts. Answers 422 when no return pack is registered for the country; the packs are listed by `declarations/eu/vat-return/packs/list`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.eu_vat_return_compute(
    country_code="countryCode",
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_jpk_v7m_generate</a>(...) -> PlJpkV7MGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate the Polish JPK_V7M(3) file (VAT declaration with evidence) for a month, per the MF schema in force since February 2026. Amounts must already be in PLN; rows are marked BFK until a KSeF integration supplies invoice numbers. Review the warnings before submitting via e-dokumenty.mf.gov.pl.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_jpk_v7m_generate(
    year=1000000,
    month=1000000,
    kod_urzedu="kodUrzedu",
    email="email",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**kod_urzedu:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**cel_zlozenia:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_vat_ue_generate</a>(...) -> PlVatUeGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the rows of the Polish recapitulative statement VAT-UE for a month: section C intra-Community supplies of goods, section D intra-Community acquisitions, section E services taxed where the customer is established. Amounts are full złoty per counterparty. The VAT-UE(5) file itself goes out from the EU sales list deadline in the calendar.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_vat_ue_generate(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_intrastat_generate</a>(...) -> PlIntrastatGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the rows of the Polish INTRASTAT declaration for a month, arrivals or dispatches, grouped by CN code, partner country, country of origin, partner VAT number, nature of transaction, transport and delivery terms. Values are whole złoty converted at the invoice rate; credit notes with goods lines are returns (code 21). Goods without a CN code are left out and named in the warnings. The IST message itself goes out from the Intrastat deadline in the calendar.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_intrastat_generate(
    year=1000000,
    month=1000000,
    flow="arrivals",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**flow:** `PlIntrastatGenerateDeclarationsRequestFlow` 
    
</dd>
</dl>

<dl>
<dd>

**transaction_nature:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_ksef_received_list</a>(...) -> PlKsefReceivedListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the invoices KSeF holds for this company as the buyer, for a window of acquisition timestamps. Each row carries the KSeF number and, when the document number matches a registered purchase invoice, the invoice it belongs to.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_ksef_received_list(
    from_=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    to=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from:** `datetime.datetime` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `datetime.datetime` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_offset:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_ksef_received_fetch</a>(...) -> PlKsefReceivedFetchDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one invoice out of KSeF by its national number. With a purchase invoice given, the KSeF number is written onto that invoice, which is what makes the purchase row of JPK_V7M carry NrKSeF instead of the BFK marker.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_ksef_received_fetch(
    ksef_number="ksefNumber",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**ksef_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_ksef_receipt</a>(...) -> PlKsefReceiptDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The UPO for a KSeF session. KSeF issues one receipt per session rather than per invoice, so the session reference number from the send is what identifies it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_ksef_receipt()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**session_reference_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_adjustments_list</a>(...) -> TaxAdjustmentsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The differences between the accounting result and the taxable profit: non-deductible expenses, income added to or left out of the tax base, extra deductible expenses, donations, losses carried forward, reliefs and tax credits. The annual corporate income tax return is built from them.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_adjustments_list(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_adjustments_create</a>(...) -> TaxAdjustmentsCreateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Records a tax adjustment of one kind for a tax year, with an optional form `code`. Answers 422 when the amount is zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_adjustments_create(
    year=1000000,
    kind="non_deductible",
    amount="121.00",
    description="description",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `TaxAdjustmentsCreateDeclarationsRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_adjustments_update</a>(...) -> TaxAdjustmentsUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the kind, code, amount or description of a recorded tax adjustment; fields left out keep their value and an empty `code` clears it. Answers 422 when the new amount is zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_adjustments_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `typing.Optional[TaxAdjustmentsUpdateDeclarationsRequestKind]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_adjustments_delete</a>(...) -> TaxAdjustmentsDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a recorded tax adjustment.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_adjustments_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_payments_list</a>(...) -> TaxPaymentsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

What the company has paid the administration towards a tax before the return is filed: payments on account, tax withheld at source by others, a final settlement, and a refund received. Returns report these on their own lines, so the amount they ask for is the balance.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_payments_list(
    tax="corporate_income_tax",
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**tax:** `TaxPaymentsListDeclarationsRequestTax` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_payments_create</a>(...) -> TaxPaymentsCreateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Records a payment made towards a tax (`tax`) of a year, and of a month when given, as an advance payment, tax withheld by others, a final settlement or a refund received. Answers 422 when the amount is zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_payments_create(
    tax="corporate_income_tax",
    year=1000000,
    kind="advance",
    amount="121.00",
    paid_on=datetime.date.fromisoformat("2026-07-01"),
    description="description",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**tax:** `TaxPaymentsCreateDeclarationsRequestTax` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `TaxPaymentsCreateDeclarationsRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**paid_on:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**reference:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_payments_update</a>(...) -> TaxPaymentsUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the kind, amount, payment date, reference or description of a recorded tax payment; fields left out keep their value and an empty `reference` clears it. Answers 422 when the new amount is zero.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_payments_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `typing.Optional[TaxPaymentsUpdateDeclarationsRequestKind]` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**paid_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**reference:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">tax_payments_delete</a>(...) -> TaxPaymentsDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a recorded tax payment.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.tax_payments_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_get</a>(...) -> AnnualAccountsGetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Whether the general meeting adopted the annual accounts and on which date, the date the accounts were prepared, and which directors signed them. The annual accounts filed with the trade register are built from these facts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_get(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_set</a>(...) -> AnnualAccountsSetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates or replaces the record of a year: whether and when the accounts were adopted, when they were prepared, whether they were audited (with the qualification flag and the auditor report date) or the auditor was not elected, the report texts and the appropriation of the result. Answers 422 when `adopted` is true without `adoptionDate`, when the adoption date is not after 31 December of the year, or when the date of preparation is after the adoption date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_set(
    year=1000000,
    adopted=True,
    date_of_preparation=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**adopted:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**date_of_preparation:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**adoption_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**audited:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**audit_report_qualified:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_not_elected:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes_text:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**management_report_text:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_report_text:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_report_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**result_to_reserves:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**result_to_loss_compensation:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**result_to_remainder:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_signatures_create</a>(...) -> AnnualAccountsSignaturesCreateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a director to the signatures of the annual accounts of the year: signed, with the date and place of signature, or not signed, with the reason. Answers 422 when no annual accounts record exists for the year (`declarations/annual-accounts/set` first), when a signed entry lacks the date or the place, or when an unsigned entry lacks the reason.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_signatures_create(
    year=1000000,
    director_name="directorName",
    director_type="managing_current",
    signed=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**director_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**director_type:** `AnnualAccountsSignaturesCreateDeclarationsRequestDirectorType` 
    
</dd>
</dl>

<dl>
<dd>

**signed:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**signed_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**signed_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**reason_not_signed:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_signatures_update</a>(...) -> AnnualAccountsSignaturesUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replaces the name, type and signing facts of a recorded director signature. Answers 422 when a signed entry lacks the date or the place of signature, or when an unsigned entry lacks the reason.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_signatures_update(
    id="id",
    director_name="directorName",
    director_type="managing_current",
    signed=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**director_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**director_type:** `AnnualAccountsSignaturesUpdateDeclarationsRequestDirectorType` 
    
</dd>
</dl>

<dl>
<dd>

**signed:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**signed_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**signed_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**reason_not_signed:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_signatures_delete</a>(...) -> AnnualAccountsSignaturesDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a recorded director signature.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_signatures_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_distributions_create</a>(...) -> AnnualAccountsDistributionsCreateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds a profit distribution decision (decision date, kind, amount, description) to the annual accounts record of the year. Answers 422 when no annual accounts record exists for the year.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_distributions_create(
    year=1000000,
    decided_on=datetime.date.fromisoformat("2026-07-01"),
    kind="dividend",
    amount="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**decided_on:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `AnnualAccountsDistributionsCreateDeclarationsRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_distributions_update</a>(...) -> AnnualAccountsDistributionsUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replaces the decision date, kind, amount and description of a recorded profit distribution.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_distributions_update(
    id="id",
    decided_on=datetime.date.fromisoformat("2026-07-01"),
    kind="dividend",
    amount="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**decided_on:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `AnnualAccountsDistributionsUpdateDeclarationsRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_distributions_delete</a>(...) -> AnnualAccountsDistributionsDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a recorded profit distribution.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_distributions_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_attachments_add</a>(...) -> AnnualAccountsAttachmentsAddDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Links a file uploaded through files/upload (its storageKey) to the annual accounts of the year as the notes, the management report, the auditor statement, the profit appropriation resolution, the approval certificate, the general data sheet, the full report as a pdf, or another document. Deposits that must carry these documents take them from here.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_attachments_add(
    year=1000000,
    kind="full_report",
    ref="ref",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `AnnualAccountsAttachmentsAddDeclarationsRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**ref:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">annual_accounts_attachments_delete</a>(...) -> AnnualAccountsAttachmentsDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the attachment from the annual accounts and deletes its file record and the stored bytes.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.annual_accounts_attachments_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">cy_td4generate</a>(...) -> CyTd4GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compute the company income tax return TD4 of a tax year from the ledger and the recorded tax adjustments: the accounting profit, the add-backs, deductions, capital allowances and losses brought forward, the chargeable income, the corporation tax at the rate of the year and the double tax relief, as the fields the company keys into TAXISnet or Tax For All. The Tax Department publishes no upload layout for the TD4; the XML is a working file.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.cy_td4generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">cy_he32generate</a>(...) -> CyHe32GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the annual return HE32 of a year: the figures the Registrar’s e-filing screens ask for (company number, registered office, made-up-to date, share capital, register of members, directors and secretary, annual general meeting date, the accounts summary), the working file, and the printed form HE32(I) filled in as a PDF for signing and for keying into the Registrar’s system, which takes the return only through its own screens.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.cy_he32generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">de_returns_generate</a>(...) -> DeReturnsGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build one of the German returns that ELSTER accepts only through a licensed ERiC transmission (E-Bilanz, Körperschaftsteuer, Gewerbesteuer with its Zerlegungserklärung, annual VAT return, Lohnsteuer-Anmeldung, Lohnsteuerbescheinigung) for the company to send through its own ELSTER-capable program. The period is the year, or YYYY-MM for the monthly Lohnsteuer-Anmeldung.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.de_returns_generate(
    rule_key="de-e-bilanz",
    period="period",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**rule_key:** `DeReturnsGenerateDeclarationsRequestRuleKey` 
    
</dd>
</dl>

<dl>
<dd>

**period:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">de_return_facts_get</a>(...) -> DeReturnFactsGetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The facts of one year that the German annual returns (Körperschaftsteuer, Gewerbesteuer, Umsatzsteuererklärung) need and the ledger does not hold: changes of shareholders, contracts with shareholders, the tax contribution account, loss carry-back, the donation carry-forward, the business premises with the municipalities for the apportionment of the trade tax, the land values or property tax and the participations for the trade tax additions and reductions, the foreign income per country for the Anlage AESt, the date of leaving the small-business scheme and the Anlage UN answers of a company seated abroad. A key that is absent has not been answered.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.de_return_facts_get(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">de_return_facts_set</a>(...) -> DeReturnFactsSetDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replace the facts of one year for the German annual returns. The returns built afterwards read them; a key left out stays unanswered.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.declarations import DeReturnFactsSetDeclarationsRequestFacts

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.de_return_facts_set(
    year=1000000,
    facts=DeReturnFactsSetDeclarationsRequestFacts(),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**facts:** `DeReturnFactsSetDeclarationsRequestFacts` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">de_deuev_generate</a>(...) -> DeDeuevGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the DEÜV notifications of a month (Anmeldung for every start, Abmeldung for every leaving, in December the Jahresmeldung for everyone employed on 31 December) as DSME records with the DBME, DBNA, DBGB and DBAN blocks of Anlage 4 in force from 2026, from the approved payroll runs and the employee record, for the company's own transmission channel.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.de_deuev_generate(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">de_beitragsnachweis_generate</a>(...) -> DeBeitragsnachweisGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the monthly contribution statement to the health insurers (Beitragsnachweis) from the payroll run: one fixed-length record BW02 per insurer, in the record layout in force from 2026, ready for the company's own transmission channel.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.de_beitragsnachweis_generate(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">dk_selskabsskat_generate</a>(...) -> DkSelskabsskatGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compute the oplysningsskema for selskaber (selskabsselvangivelsen) of an income year from the ledger and the recorded tax adjustments: accounting result before tax, tax adjustments, losses carried forward, taxable income, the 22 % corporation tax, reliefs and the balance, as the rubrikker the company keys into TastSelv Selskabsskat (DIAS). Skatteforvaltningen publishes no file format for the return; the XML is a working file.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.dk_selskabsskat_generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ee_employment_register_send</a>(...) -> EeEmploymentRegisterSendDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send one employment register (töötamise register) entry for an employment contract to e-MTA over X-tee: the start of work, or its end with the reason recorded on the contract.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ee_employment_register_send(
    contract_id="contractId",
    event="start",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**contract_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**event:** `EeEmploymentRegisterSendDeclarationsRequestEvent` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">es_verifactu_declaracion_responsable</a>() -> EsVerifactuDeclaracionResponsableDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Nordlet's declaración responsable for its VERI*FACTU invoicing system (Orden HAC/1177/2024, art. 15), as a PDF and as plain text.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.es_verifactu_declaracion_responsable()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ie_ct1generate</a>(...) -> IeCt1GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the Form CT1 of an accounting year as the ROS version 26 XML and the accompanying financial statements as inline XBRL on the FRS 102 Irish Extension 2026 taxonomy Revenue accepts, both from the ledger, the recorded tax adjustments, the annual accounts record and the officers, for upload through the company’s own ROS account. Says whether the company is above the iXBRL deferral limits (balance sheet total €4.4 million, turnover €8.8 million, 50 employees).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ie_ct1generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ie_b1generate</a>(...) -> IeB1GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the working paper for the Form B1 annual return of a financial year - company details, registered office, directors and secretary from Account → Officers, the members from Account → Shareholders, the issued share capital and the figures of the financial statements - in the order the CORE screens ask for them. The CRO publishes no file format for the B1, so it is keyed into CORE.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ie_b1generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">it_sdi_purchase_send</a>(...) -> ItSdiPurchaseSendDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the TD16-TD19 integration document for a registered purchase invoice and send it to the Sistema di Interscambio. Since July 2022 a purchase from a supplier established abroad is reported this way instead of the esterometro. The Italian VAT rate to self-assess is a judgement about the supply: pass vatRatePercent unless the purchase lines already carry it, otherwise the request is refused rather than guessed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.it_sdi_purchase_send(
    purchase_invoice_id="purchaseInvoiceId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**purchase_invoice_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tipo_documento:** `typing.Optional[ItSdiPurchaseSendDeclarationsRequestTipoDocumento]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">it_sdi_purchase_preview</a>(...) -> ItSdiPurchasePreviewDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render the TD16-TD19 integration document for a registered purchase invoice without sending it, so the rate and the document type can be checked first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.it_sdi_purchase_preview(
    purchase_invoice_id="purchaseInvoiceId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**purchase_invoice_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tipo_documento:** `typing.Optional[ItSdiPurchasePreviewDeclarationsRequestTipoDocumento]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_saft_send</a>(...) -> LtSaftSendDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Upload the SAF-T file to i.SAF-T over the iSAFTUploaderService web service and start its processing. The file, the case reference and the status are kept as a declaration submission (submissionId), whose outcome Nordlet then checks with i.SAF-T. The submission itself is confirmed separately, because after confirmation the file can no longer be corrected. A range and data type already sent is sent again only with amend: true.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_saft_send(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**data_type:** `typing.Optional[LtSaftSendDeclarationsRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**confirm:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**amend:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_sd_ffdata</a>(...) -> LtSdFfdataDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render the Sodra 1-SD or 2-SD notice for the contracts starting or ending in the range as an .ffdata document for EDAS.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_sd_ffdata(
    type="1-SD",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `LtSdFfdataDeclarationsRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**manager_full_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**preparator_details:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">lt_pln204ffdata</a>(...) -> LtPln204FfdataDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Render the annual corporate income tax return PLN204 as an .ffdata document, including the PLN204S and PLN204Z annexes, from the ledger and the tax adjustments recorded for that year.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.lt_pln204ffdata(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">mt_company_tax_generate</a>(...) -> MtCompanyTaxGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compute the company income tax return and self-assessment of a year of assessment from the ledger and the recorded tax adjustments: the accounting profit before tax, the add-backs and deductions, the approved donations, capital allowances and losses carried forward, the chargeable income, the 35 % charge, the relief against the tax and the allocation of the distributable profit to the five tax accounts. The Malta Tax and Customs Administration issues the return as a personalised spreadsheet to the registered tax practitioner and publishes no layout, so the XML is a working file and the figures are keyed into that spreadsheet.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.mt_company_tax_generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">mt_annual_return_generate</a>(...) -> MtAnnualReturnGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the annual return of a year: the company number, registered office and made-up-to date, the share capital, the register of members, the directors and the company secretary and the accounts summary, as the figures the Malta Business Registry asks for on its own screens, plus the printed Annual Return Form of the Seventh Schedule filled in as a PDF for signing.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.mt_annual_return_generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_jpk_fa_generate</a>(...) -> PlJpkFaGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate JPK_FA(4), the on-demand structure with every sales invoice issued in a period, its VAT bases per rate and one row per invoice line. Filed only when the tax office asks for it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_jpk_fa_generate(
    date_from=datetime.date.fromisoformat("2026-07-01"),
    date_to=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date_from:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_jpk_kr_generate</a>(...) -> PlJpkKrGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate JPK_KR(1), the on-demand structure with the chart of accounts and its opening balances and turnover, the journal and the double entries behind it. Filed only when the tax office asks for it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_jpk_kr_generate(
    date_from=datetime.date.fromisoformat("2026-07-01"),
    date_to=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date_from:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_jpk_mag_generate</a>(...) -> PlJpkMagGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate JPK_MAG(2), the on-demand structure with the warehouse documents of one warehouse: goods received from outside (PZ) or internally (PW) and issued to a customer (WZ) or internally (RW). Filed only when the tax office asks for it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_jpk_mag_generate(
    date_from=datetime.date.fromisoformat("2026-07-01"),
    date_to=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date_from:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_pit11generate</a>(...) -> PlPit11GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate PIT-11(29) for every person on the payroll of one year: the pay, the deductible costs, the advance withheld and the social and health contributions taken off it. One document per person, because that is how the form is filed, addressed to the tax office of the place of residence of that person (employee field plKodUrzedu); a person without that code is refused with 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_pit11generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_cit8generate</a>(...) -> PlCit8GenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate CIT-8(34), the annual corporate income tax return, from the ledger of the year and the recorded tax adjustments. The tax office code and the small-taxpayer setting come from the e-Deklaracje compliance settings, the seat address from the JPK gateway settings. Names the annexes the figures would need, which are not produced.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_cit8generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_zus_dra_compute</a>(...) -> PlZusDraComputeDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Compute the monthly ZUS DRA settlement from the payroll run of one month: the pension, disability, sickness, accident and health insurance contributions and the Labour Fund, Solidarity Fund and guaranteed benefits fund charges, each split between the insured person and the payer. The amounts are carried into Płatnik or ePłatnik by hand.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_zus_dra_compute(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_zus_dra_kedu</a>(...) -> PlZusDraKeduDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the KEDU file for one month: the ZUS DRA settlement and one ZUS RCA report per person on the payroll, in the schema kedu_5_4 that Płatnik and ePłatnik import. The payer REGON, short name and declaration deadline code come from the ZUS compliance settings; the insurance title code and working time of each person from the employee record.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_zus_dra_kedu(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">pl_zus_dra_pdf</a>(...) -> PlZusDraPdfDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Fill the published ZUS DRA form for one month and return it as a PDF. The amounts, the payer identity and the deadline code are the same ones the KEDU file carries; blocks the payroll does not hold (paid benefits, bridging pensions, income declaration of a self-paying person) stay empty.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.pl_zus_dra_pdf(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ro_etransport_build</a>(...) -> RoEtransportBuildDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the RO e-Transport declaration for an issued waybill: goods with their tariff codes and masses, the commercial partner, the route and the vehicle. The XML follows the ANAF eTransport v2 schema and is kept as a file on the waybill. Anything listed in blockers has to be filled in before /etransport/send will accept it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ro_etransport_build(
    waybill_id="waybillId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**waybill_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ro_etransport_submit</a>(...) -> RoEtransportSubmitDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Hand the RO e-Transport declaration for an issued waybill to ANAF under the SPV OAuth token in compliance settings, and return the upload index the UIT is read back with. Answers 422 while any field the ANAF validator requires is still missing.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ro_etransport_submit(
    waybill_id="waybillId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**waybill_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">ro_etransport_status</a>(...) -> RoEtransportStatusDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read the outcome of an e-Transport declaration from ANAF by its upload index, under the SPV OAuth token in compliance settings. Returns the UIT code once the declaration validates.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.ro_etransport_status(
    reference="reference",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**reference:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">li_lohndeklaration_generate</a>(...) -> LiLohndeklarationGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the annual wage declaration (Lohndeklaration) to the AHV-IV-FAK from the approved payroll runs of the year as the CSV that AHVeasy imports under Lohndeklaration → CSV-Import der Lohndaten: one row per employee with the 18 columns of the AHVeasy template, the AHV-liable wage and the ALV wage.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.li_lohndeklaration_generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">li_lohnlisten_generate</a>(...) -> LiLohnlistenGenerateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the annual wage list (Lohnliste) of a Liechtenstein employer from the approved payroll runs of the year as the XLSX file the tax administration's eLohnausweis / eLohnlisten application imports: one row per employee with PEID, name, birth date, address, gross wage, wage tax withheld and the settlement period.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.li_lohnlisten_generate(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">configs_list</a>(...) -> ConfigsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the filing systems the company can configure: those of the company country (or of `country` when given), the EU-wide systems and the cross-border e-invoicing systems `it_sdi`, `pl_ksef` and `ro_efactura`. Each row carries the stored values, with a secret or certificate field shown as `__secret_set__` and the fields taken from the company profile filled from it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.configs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country:** `typing.Optional[str]` — List the systems of this country instead of the company country
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">configs_update</a>(...) -> ConfigsUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stores the settings of one filing system for the company, merging the given fields into the stored ones. A secret or certificate value is encrypted before it is stored, an empty string clears a field, and `__secret_set__` leaves a stored secret unchanged. Answers 422 for an unknown system.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.configs_update(
    system="system",
    config={
        "key": "value"
    },
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**system:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**config:** `typing.Dict[str, str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">certificates_upload</a>(...) -> CertificatesUploadDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stores a PEM certificate, a PEM private key or a PKCS#12 bundle (base64 in `content`, opened with `passphrase` when it needs one) in the settings of the filing system and replaces the earlier upload of the same kind; for a PEM certificate the fingerprint, subject, issuer and validity dates are recorded. Answers 422 when the system is unknown or does not authenticate with a certificate. Returns the full certificate list of the company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.certificates_upload(
    system="system",
    file_name="fileName",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**system:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**file_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` — Base64-encoded PEM or PKCS#12 file
    
</dd>
</dl>

<dl>
<dd>

**passphrase:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">certificates_list</a>() -> CertificatesListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the certificates and private keys stored for the filing systems of the company, ordered by system and field, each with its validity facts and health (`ok`, `expiring`, `expired` or `unknown`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.certificates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">certificates_delete</a>(...) -> CertificatesDeleteDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the certificate or the private key (`fieldKey`) of a filing system from the settings of the company and from the certificate list, and returns the remaining certificates.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.certificates_delete(
    system="system",
    field_key="certificate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**system:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**field_key:** `CertificatesDeleteDeclarationsRequestFieldKey` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">automation_list</a>() -> AutomationListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the filing deadlines Nordlet can file by itself for the country of the company: for each, whether automatic filing is switched on, whether the rule applies to the company profile, whether its filing system is configured, the state of its certificate and whether it would go to the test or the production service.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.automation_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">automation_update</a>(...) -> AutomationUpdateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Switches automatic filing of one deadline on or off for the company and returns the list of `declarations/automation/list`. Answers 422 when the deadline is not one Nordlet files, or when switching on while the filing system is connected to the test service of the administration (unless the company is a sandbox), is not configured, or has no valid certificate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.automation_update(
    rule_key="ruleKey",
    enabled=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**rule_key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**enabled:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">submissions_retry</a>(...) -> SubmissionsRetryDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Sends a submission that is still in status `generated` through its filing system once more, with the stored file or, when none was stored yet, a freshly generated one, and returns the updated submission. Answers 409 when the submission is already submitted, accepted or rejected.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.submissions_retry(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">submissions_create</a>(...) -> SubmissionsCreateDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the Lithuanian i.SAF register file of a month (`dataType` F both registers, S sale invoices only, P purchase invoices only), stores it and creates a submission in status `generated` for the obligation `lt-isaf`, the only obligation accepted. The XML alone comes from `declarations/lt/isaf/generate`; the submission is moved on with `declarations/submissions/mark`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.submissions_create(
    obligation="lt-isaf",
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**obligation:** `SubmissionsCreateDeclarationsRequestObligation` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**data_type:** `typing.Optional[SubmissionsCreateDeclarationsRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">submissions_mark</a>(...) -> SubmissionsMarkDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Records by hand that a submission was sent, accepted or rejected, with the reference and message of the administration when given. The allowed moves are `generated` to `submitted` and `submitted` to `accepted` or `rejected`; any other move answers 409. A submission without a transport system is marked as sent manually.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.submissions_mark(
    id="id",
    status="submitted",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `SubmissionsMarkDeclarationsRequestStatus` 
    
</dd>
</dl>

<dl>
<dd>

**external_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**message:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">submissions_list</a>(...) -> SubmissionsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the declaration submissions of the company, newest first, filterable by `obligation`, `status`, `periodYear` and `periodMonth` and sortable by `createdAt` or `periodYear`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.submissions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SubmissionsListDeclarationsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SubmissionsListDeclarationsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ledger
<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">accounts_list</a>(...) -> AccountsListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's chart of accounts. Filterable by `code`, `name`, `type` and `isPostable`; sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.accounts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AccountsListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AccountsListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">accounts_create</a>(...) -> AccountsCreateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds an account to the company's chart of accounts. `parentId` must name an account of the same company. Answers 409 when an account with the same `code` already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.accounts_create(
    code="code",
    name="name",
    type="asset",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `AccountsCreateLedgerRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_postable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">accounts_update</a>(...) -> AccountsUpdateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the name, parent or postability of an account; the code and type cannot be changed. An account cannot be its own parent.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.accounts_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**parent_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_postable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">accounts_apply_template</a>() -> AccountsApplyTemplateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds the accounts of the company's chart template that the chart does not have yet (an account whose code already exists is not replaced) and sets the parent links the template defines. Returns the number of accounts in the chart afterwards.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.accounts_apply_template()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">accounts_switch_chart</a>() -> AccountsSwitchChartLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replaces the seeded chart with the chart template of the company country (the Romanian general chart for a company registered in Romania, the Estonian e-arveldaja chart for a company registered in Estonia, the Lithuanian standard chart otherwise) and switches the posting defaults with it. Answers 409 when the company already uses that chart, has journal entries, holds accounts created by hand, or has settings that name an account the new chart does not have.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.accounts_switch_chart()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">periods_list</a>(...) -> PeriodsListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's accounting periods with their `open` or `locked` status. Filterable by `year`, `month` and `status`; sortable by `year` and `month`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.periods_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[PeriodsListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PeriodsListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">periods_lock</a>(...) -> PeriodsLockLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Locks the month so that postings dated in it are refused with 409 (`ledger/journal/transactions/create`, `cash/orders/create` and `cash/expense-reports/create` among them). Before locking a month that is not locked yet, posts the pending ratable revenue recognition tranches scheduled up to the month end and emits `revenue_recognition.posted` when there were any; when the month is the company's fiscal year end and no year-end close is posted for that year, posts the year-end close that moves the income and expense balances of the fiscal year to the retained earnings account (posting rule `closing.retainedEarnings`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.periods_lock(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">periods_unlock</a>(...) -> PeriodsUnlockLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Opens the month for posting again. When the month is the company's fiscal year end and a year-end close is posted for it, posts a reversal of that close dated the same day.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.periods_unlock(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">journal_transactions_list</a>(...) -> JournalTransactionsListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists journal transactions with the partner name. Filterable by `date`, `status`, `documentType`, `partnerId` and `documentId`; sortable by `date` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.journal_transactions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[JournalTransactionsListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[JournalTransactionsListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_centers_create</a>(...) -> CostCentersCreateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a cost center, optionally inside a cost center group. Answers 409 when the `code` is already used.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_centers_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_centers_update</a>(...) -> CostCentersUpdateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the name, group or active flag of a cost center. An inactive cost center is refused on new manual journal entries (`ledger/journal/transactions/create` answers 422).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_centers_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_centers_list</a>(...) -> CostCentersListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists cost centers with their group name. Filterable by `code`, `name`, `isActive` and `groupId`; sortable by `code`, `name` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_centers_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[CostCentersListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[CostCentersListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_center_groups_create</a>(...) -> CostCenterGroupsCreateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a cost center group. Answers 409 when the `code` is already used.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_center_groups_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_center_groups_update</a>(...) -> CostCenterGroupsUpdateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the code or name of a cost center group. Answers 409 when the new code is already used.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_center_groups_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_center_groups_delete</a>(...) -> CostCenterGroupsDeleteLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a cost center group. Answers 409 while cost centers are still assigned to it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_center_groups_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">cost_center_groups_list</a>(...) -> CostCenterGroupsListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists cost center groups. Filterable and sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.cost_center_groups_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[CostCenterGroupsListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[CostCenterGroupsListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">posting_rules_list</a>() -> PostingRulesListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists every posting rule with its default account code on the company's chart template, the account code in effect and whether the company has overridden it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.posting_rules_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">posting_rules_update</a>(...) -> PostingRulesUpdateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Overrides the account code of one or more posting rules; an `accountCode` of null removes the override and the chart default applies again. Every code given must be a postable account of the company's chart, else 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.ledger import PostingRulesUpdateLedgerRequestRulesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.posting_rules_update(
    rules=[
        PostingRulesUpdateLedgerRequestRulesItem(
            key="sales.receivable",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**rules:** `typing.List[PostingRulesUpdateLedgerRequestRulesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">owners_create</a>(...) -> OwnersCreateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds an owner of the company. `equityAccountCode` defaults to the share capital account of the company's chart; a code that is not in the chart of accounts answers 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.owners_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**equity_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_type:** `typing.Optional[OwnersCreateLedgerRequestSharesType]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_acquisition_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**withholding_tax_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_liability:** `typing.Optional[OwnersCreateLedgerRequestPartnerLiability]` 
    
</dd>
</dl>

<dl>
<dd>

**special_balance_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_balance_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[OwnersCreateLedgerRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">owners_update</a>(...) -> OwnersUpdateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the fields of an owner. An `equityAccountCode` that is not in the chart of accounts answers 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.owners_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**equity_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_type:** `typing.Optional[OwnersUpdateLedgerRequestSharesType]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_acquisition_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**withholding_tax_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_liability:** `typing.Optional[OwnersUpdateLedgerRequestPartnerLiability]` 
    
</dd>
</dl>

<dl>
<dd>

**special_balance_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**supplementary_balance_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[OwnersUpdateLedgerRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">owners_delete</a>(...) -> OwnersDeleteLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes an owner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.owners_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">owners_list</a>(...) -> OwnersListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's owners. Filterable by `name` and `code`; sortable by `name` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.owners_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[OwnersListLedgerRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[OwnersListLedgerRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">journal_transactions_get</a>(...) -> JournalTransactionsGetLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns a journal transaction with its entries, ordered by account code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.journal_transactions_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">journal_transactions_create</a>(...) -> JournalTransactionsCreateLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Posts a manual journal transaction (`documentType` `manual`, status `posted`) in the company's base currency. Every `accountCode` must be a postable account of the chart, cost centers must exist and be active, projects must exist, and the debits must equal the credits. Answers 422 for an amount with more than two decimals, for a `currency` other than the base currency and for an inactive cost center, and 409 when the accounting period of `date` is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.ledger import JournalTransactionsCreateLedgerRequestEntriesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.journal_transactions_create(
    date=datetime.date.fromisoformat("2026-07-01"),
    entries=[
        JournalTransactionsCreateLedgerRequestEntriesItem(
            account_code="accountCode",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**entries:** `typing.List[JournalTransactionsCreateLedgerRequestEntriesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">statement_rows_schemes</a>() -> StatementRowsSchemesLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The rows or codes of each return or registry deposit of the company country that are filled from account balances. Accounts fall into a row by the layout defaults for the standard chart of accounts unless mapped under Account → Statement rows.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.statement_rows_schemes()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">statement_rows_list</a>(...) -> StatementRowsListLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Every postable account of the company with the row of `scheme` it falls into, by a mapping (`ledger/statement-rows/set`) or by the layout default, and the amount it carries there: the balance up to `toDate` on a balance-sheet row, the movement from `fromDate` to `toDate` on an income-statement row. `toDate` defaults to today and `fromDate` to 1 January of that year. `rows` holds the row totals and `unmapped` the accounts with a balance but no row.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.statement_rows_list(
    scheme="scheme",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**scheme:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">statement_rows_set</a>(...) -> StatementRowsSetLedgerResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

A mapping on a code prefix covers every account whose code starts with it; the longest matching prefix wins. An empty rowCode removes the mapping so the layout default applies again.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.statement_rows_set(
    scheme="scheme",
    account_code="accountCode",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**scheme:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**account_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**row_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Officers
<details><summary><code>client.officers.<a href="src/nordlet/officers/client.py">list</a>() -> ListOfficersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Directors, board members, the company secretary, representatives and liquidators, with their personal identifier, appointment and resignation dates and whether they sign the annual accounts. Annual returns and registry deposits are built from this register.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.officers.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.officers.<a href="src/nordlet/officers/client.py">create</a>(...) -> CreateOfficersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Add an officer to the company's register (`officers/list`); `signsAccounts` defaults to true. Refused with 422 when `resignedOn` is before `appointedOn`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.officers.create(
    name="name",
    role="director",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `CreateOfficersRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**personal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**appointed_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**power_notary:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**resigned_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**signs_accounts:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.officers.<a href="src/nordlet/officers/client.py">update</a>(...) -> UpdateOfficersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replace the recorded data of an officer; every field is written as sent, so a field left out is cleared and `signsAccounts` falls back to true. Refused with 422 when `resignedOn` is before `appointedOn`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.officers.update(
    id="id",
    name="name",
    role="director",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `UpdateOfficersRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**personal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**appointed_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**power_notary:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**resigned_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**signs_accounts:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.officers.<a href="src/nordlet/officers/client.py">delete</a>(...) -> DeleteOfficersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove an officer from the company's register.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.officers.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## PlatformSellers
<details><summary><code>client.platform_sellers.<a href="src/nordlet/platform_sellers/client.py">list</a>(...) -> ListPlatformSellersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Individuals and entities that sell goods, rent out property or transport, or perform personal services through the platform the company operates. The yearly DAC7 report is built from them.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.platform_sellers.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListPlatformSellersRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListPlatformSellersRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.platform_sellers.<a href="src/nordlet/platform_sellers/client.py">get</a>(...) -> GetPlatformSellersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one platform seller with its activities, ordered by year.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.platform_sellers.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.platform_sellers.<a href="src/nordlet/platform_sellers/client.py">create</a>(...) -> CreatePlatformSellersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a seller on the company's platform for the DAC7 report: an `individual` (first and last name required) or an `entity` (`entityName` required), with its `activities` per year and quarter. An `immovable_property` activity needs `propertyAddress`; property address, type and rented days on any other kind of activity are refused. These checks answer 422; a `partnerId` that does not exist answers 404. The report is built from the sellers with `declarations/eu/dac7/preview` and `declarations/eu/dac7/xml`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.platform_sellers import CreatePlatformSellersRequestAddress

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.platform_sellers.create(
    kind="individual",
    address=CreatePlatformSellersRequestAddress(
        country_code="countryCode",
    ),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**kind:** `CreatePlatformSellersRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `CreatePlatformSellersRequestAddress` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**middle_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**entity_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tax_residences:** `typing.Optional[typing.List[CreatePlatformSellersRequestTaxResidencesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**business_registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_city:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**account_holder_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**government_entity:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**listed_entity:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**permanent_establishments:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**activities:** `typing.Optional[typing.List[CreatePlatformSellersRequestActivitiesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.platform_sellers.<a href="src/nordlet/platform_sellers/client.py">update</a>(...) -> UpdatePlatformSellersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replace a platform seller's details and all of its activities with the ones given, under the same checks as `platform-sellers/create`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.platform_sellers import UpdatePlatformSellersRequestAddress

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.platform_sellers.update(
    id="id",
    kind="individual",
    address=UpdatePlatformSellersRequestAddress(
        country_code="countryCode",
    ),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `UpdatePlatformSellersRequestKind` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `UpdatePlatformSellersRequestAddress` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**middle_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**entity_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**tax_residences:** `typing.Optional[typing.List[UpdatePlatformSellersRequestTaxResidencesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**business_registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_city:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**account_holder_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**government_entity:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**listed_entity:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**permanent_establishments:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**activities:** `typing.Optional[typing.List[UpdatePlatformSellersRequestActivitiesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.platform_sellers.<a href="src/nordlet/platform_sellers/client.py">delete</a>(...) -> DeletePlatformSellersResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark a platform seller as deleted. It leaves the lists and the DAC7 report.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.platform_sellers.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## migration
<details><summary><code>client.migration.<a href="src/nordlet/migration/client.py">books_validate</a>(...) -> BooksValidateMigrationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Runs every check the import runs (accounts, partners, balances, open invoices, assets, stock) and returns the same summary and warnings, then rolls everything back. Nothing is stored.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.migration.books_validate(
    cutover_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cutover_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**source:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts:** `typing.Optional[typing.List[BooksValidateMigrationRequestAccountsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**partners:** `typing.Optional[typing.List[BooksValidateMigrationRequestPartnersItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.Optional[typing.List[BooksValidateMigrationRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**opening_balances:** `typing.Optional[BooksValidateMigrationRequestOpeningBalances]` 
    
</dd>
</dl>

<dl>
<dd>

**journal:** `typing.Optional[typing.List[BooksValidateMigrationRequestJournalItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_receivables:** `typing.Optional[typing.List[BooksValidateMigrationRequestOpenReceivablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_payables:** `typing.Optional[typing.List[BooksValidateMigrationRequestOpenPayablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**asset_groups:** `typing.Optional[typing.List[BooksValidateMigrationRequestAssetGroupsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_assets:** `typing.Optional[typing.List[BooksValidateMigrationRequestFixedAssetsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**stock:** `typing.Optional[typing.List[BooksValidateMigrationRequestStockItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.migration.<a href="src/nordlet/migration/client.py">books_import</a>(...) -> BooksImportMigrationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Brings a company over from another system in one call: chart of accounts, partners, items, opening balances (or the full journal history), open customer and supplier invoices, fixed assets with their accumulated depreciation, and stock on hand. The whole package is written in one database transaction - if any row fails, nothing is stored.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.migration.books_import(
    cutover_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cutover_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**source:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts:** `typing.Optional[typing.List[BooksImportMigrationRequestAccountsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**partners:** `typing.Optional[typing.List[BooksImportMigrationRequestPartnersItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.Optional[typing.List[BooksImportMigrationRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**opening_balances:** `typing.Optional[BooksImportMigrationRequestOpeningBalances]` 
    
</dd>
</dl>

<dl>
<dd>

**journal:** `typing.Optional[typing.List[BooksImportMigrationRequestJournalItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_receivables:** `typing.Optional[typing.List[BooksImportMigrationRequestOpenReceivablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_payables:** `typing.Optional[typing.List[BooksImportMigrationRequestOpenPayablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**asset_groups:** `typing.Optional[typing.List[BooksImportMigrationRequestAssetGroupsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_assets:** `typing.Optional[typing.List[BooksImportMigrationRequestFixedAssetsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**stock:** `typing.Optional[typing.List[BooksImportMigrationRequestStockItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## assets
<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">settings_get</a>() -> SettingsGetAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the company's fixed asset setting `autoDepreciation`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">settings_update</a>(...) -> SettingsUpdateAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Turn automatic depreciation on or off. When it is on, the scheduler posts the previous month's depreciation for the company once a day, as `assets/depreciation/post` does.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.settings_update(
    auto_depreciation=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**auto_depreciation:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">groups_create</a>(...) -> GroupsCreateAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an asset group: the asset, accumulated depreciation and depreciation expense accounts its assets are posted to, and an optional default useful life in months. `expenseAccountCode` defaults to the chart's depreciation expense account; each account must exist and be postable (422). A duplicate code is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.groups_create(
    code="code",
    name="name",
    asset_account_code="assetAccountCode",
    depreciation_account_code="depreciationAccountCode",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**asset_account_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**depreciation_account_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**default_useful_life_months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">groups_list</a>(...) -> GroupsListAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the asset groups; filterable and sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.groups_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[GroupsListAssetsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[GroupsListAssetsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_create</a>(...) -> AssetsCreateAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a fixed asset in a group with its acquisition date and cost, salvage value, useful life in months (defaults to the group's default; 422 when neither is set) and depreciation start date (defaults to the acquisition date). The salvage value must be below the acquisition cost (422); a duplicate code is refused with 409. Depreciation is posted with `assets/depreciation/post`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_create(
    group_id="groupId",
    code="code",
    name="name",
    acquisition_date=datetime.date.fromisoformat("2026-07-01"),
    acquisition_cost="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_cost:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**depreciation_start_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**salvage_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**useful_life_months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[AssetsCreateAssetsRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_update</a>(...) -> AssetsUpdateAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change an asset that has no posted depreciation yet: group, code, name, dates, cost, salvage value, useful life, notes or documents. Refused with 409 once depreciation is posted or the asset is disposed, and with 422 when the salvage value would reach the acquisition cost; a duplicate code is 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**group_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**depreciation_start_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_cost:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**salvage_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**useful_life_months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[AssetsUpdateAssetsRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_input_vat</a>(...) -> AssetsInputVatAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record the input VAT facts of a capital good that the annual VAT return needs for the adjustment of the deduction over the adjustment period (Article 187 of the VAT Directive, § 15a UStG): the input VAT on the acquisition, the date of first use, the share of use for deductible turnover at first use, whether it is land or a building (ten-year period instead of five), and every later year in which the share changed or the good was sold or withdrawn. Allowed also after depreciation has been posted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.assets import AssetsInputVatAssetsRequestInputVatUseChangesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_input_vat(
    id="id",
    input_vat_real_estate=True,
    input_vat_use_changes=[
        AssetsInputVatAssetsRequestInputVatUseChangesItem(
            year=1000000,
            percent="121.00",
            reason="use_change",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**input_vat_real_estate:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**input_vat_use_changes:** `typing.List[AssetsInputVatAssetsRequestInputVatUseChangesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**input_vat_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**input_vat_first_use_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**input_vat_deductible_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_get</a>(...) -> AssetsGetAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one fixed asset with its totals (cost including modernisations, accumulated depreciation, net book value, total life in months), its input VAT facts and its disposal.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_list</a>(...) -> AssetsListAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the fixed assets; filterable by `code`, `name`, `groupId`, `status`, `acquisitionDate`, `acquisitionCost` and `accumulatedDepreciation`, sortable by `code`, `name`, `acquisitionDate` and `acquisitionCost`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AssetsListAssetsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AssetsListAssetsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_modernize</a>(...) -> AssetsModernizeAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a modernisation of a fixed asset: `amount` is added to its cost and `addedLifeMonths` to its useful life from the month of `date` on, and the remaining depreciable value is spread over the months left. Refused with 422 when the asset is disposed or when no depreciation month would be left (give `addedLifeMonths` of at least 1); a fully depreciated asset becomes active again.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_modernize(
    id="id",
    date=datetime.date.fromisoformat("2026-07-01"),
    amount="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**added_life_months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">assets_dispose</a>(...) -> AssetsDisposeAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Dispose of a fixed asset (sold, scrapped or written off). Removes its cost and accumulated depreciation, books the net book value as a disposal loss and the proceeds as a disposal gain (posting rules assets.disposalLoss, assets.disposalGain, assets.disposalProceeds), and stops its depreciation. Depreciation must be posted for every month before the disposal month.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.assets_dispose(
    id="id",
    date=datetime.date.fromisoformat("2026-07-01"),
    reason="sold",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `AssetsDisposeAssetsRequestReason` 
    
</dd>
</dl>

<dl>
<dd>

**proceeds:** `typing.Optional[str]` — Sale price excluding VAT; 0 when scrapped or written off
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">depreciation_preview</a>(...) -> DepreciationPreviewAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Preview what `assets/depreciation/post` would post for a month: per active asset the amount and the months it covers, earlier unposted months included, and whether the month is already posted. Nothing is written.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.depreciation_preview(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">depreciation_post</a>(...) -> DepreciationPostAssetsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Post the depreciation of a month: one journal entry dated the last day of the month that debits each group's expense account and credits its accumulated depreciation account, for every active asset whose depreciation has started, covering that month and any earlier month not yet posted. Each month's amount is the remaining depreciable value (cost plus modernisations less salvage value less accumulated depreciation) divided by the months left; an asset whose life or value is used up becomes `fully_depreciated`. Answers 409 when the period is locked, and `journalTransactionId` null when nothing is due.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.depreciation_post(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## hr
<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">positions_create</a>(...) -> PositionsCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a job position with an optional code and name translations, for use in `hr/contracts/create`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.positions_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**translations:** `typing.Optional[typing.Dict[str, PositionsCreateHrRequestTranslationsValue]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">positions_update</a>(...) -> PositionsUpdateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the code, name or translations of a position; a null `translations` removes them.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.positions_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**translations:** `typing.Optional[typing.Dict[str, typing.Optional[PositionsUpdateHrRequestTranslationsValue]]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">positions_list</a>(...) -> PositionsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's positions; filterable and sortable by `name` and `code`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.positions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[PositionsListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PositionsListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_create</a>(...) -> EmployeesCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates an employee record. `payrollOptions` holds the country-specific settings the payroll engine reads for the person (see `hr/employees/fields`); `applyAllowance` defaults to true and `pensionAccumulation` to false.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_create(
    first_name="firstName",
    last_name="lastName",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**first_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**last_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**personal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[EmployeesCreateHrRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**social_insurance_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**social_insurance_start:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**hire_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**apply_allowance:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**allowance_override:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pension_accumulation:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**payroll_options:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.List[EmployeesCreateHrRequestAttributesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_update</a>(...) -> EmployeesUpdateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of an employee; a null clears the fields that allow it (code, personal code, birth date, contact details, address, IBAN, social insurance number and start, hire date, notes). `status` and `terminationDate` are set here too.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**first_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**personal_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**birth_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[EmployeesUpdateHrRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**social_insurance_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**social_insurance_start:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**hire_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**apply_allowance:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**allowance_override:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pension_accumulation:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**payroll_options:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.List[EmployeesUpdateHrRequestAttributesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**termination_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[EmployeesUpdateHrRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_get</a>(...) -> EmployeesGetHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads one employee.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_fields</a>() -> EmployeesFieldsHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Attributes a filing of the company country needs about a person that the shared employee record does not carry, such as the sex and place of birth an Italian income certificate asks for. Their values are kept in the payrollOptions of the employee.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_fields()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_list</a>(...) -> EmployeesListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the employees that are not deleted; filterable by `firstName`, `lastName`, `code`, `status` and `email`, sortable by `lastName`, `code` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[EmployeesListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[EmployeesListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_delete</a>(...) -> EmployeesDeleteHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Marks the employee deleted; the record stays and no longer appears in lists or payroll runs. `hr/employees/anonymize` also blanks the personal data.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_anonymize</a>(...) -> EmployeesAnonymizeHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Replaces the name with a placeholder and removes personal code, birth date, contact details, address, bank account, social-insurance number, notes and sick-leave reasons. Payroll and contract rows stay linked to the record for the statutory retention period.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_anonymize(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">contracts_create</a>(...) -> ContractsCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates an employment contract for an employee. A `permanent` contract takes no `endDate` and a `fixed_term` one requires it; the number comes from `contractNo` or, with `agreementId`, from the employee's agreement; `workHours` defaults by `salaryType`. Answers 422 when the end date is before the start, and 409 when the employee already has a contract overlapping the period (end it with `hr/contracts/end` first) or the contract number already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.contracts_create(
    employee_id="employeeId",
    start_date=datetime.date.fromisoformat("2026-07-01"),
    base_salary="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**start_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**base_salary:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**position_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**department_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**schedule_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**agreement_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**contract_no:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ContractsCreateHrRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**salary_type:** `typing.Optional[ContractsCreateHrRequestSalaryType]` 
    
</dd>
</dl>

<dl>
<dd>

**work_hours:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">contracts_end</a>(...) -> ContractsEndHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Ends a contract on `endDate` with an optional reason. Answers 422 when the end date is before the contract start.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.contracts_end(
    id="id",
    end_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**end_reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">contracts_list</a>(...) -> ContractsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists employment contracts; filterable by `employeeId`, `agreementId`, `status` and `contractNo`, sortable by `startDate` and `contractNo`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.contracts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ContractsListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ContractsListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">leave_balances_set</a>(...) -> LeaveBalancesSetHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates or replaces the leave entitlement of an employee for a year; `usedDays` is kept unless given (0 on a new row) and `remainingDays` is the entitled days less the used ones.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.leave_balances_set(
    employee_id="employeeId",
    year=1000000,
    entitled_days="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**entitled_days:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**used_days:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">leave_balances_list</a>(...) -> LeaveBalancesListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists leave balances, narrowed to an employee and/or a year when given, oldest year first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.leave_balances_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">incapacity_certificates_create</a>(...) -> IncapacityCertificatesCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Records a sick-leave certificate of an employee. Answers 422 when `toDate` is before `fromDate`. `payroll/runs/create` warns when a certificate covers working days of a month that has no timesheet.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.incapacity_certificates_create(
    employee_id="employeeId",
    number="number",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">incapacity_certificates_list</a>(...) -> IncapacityCertificatesListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists incapacity certificates; filterable by `employeeId` and `number`, sortable by `fromDate` and `number`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.incapacity_certificates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[IncapacityCertificatesListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[IncapacityCertificatesListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">per_diem_rates_create</a>(...) -> PerDiemRatesCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds the company's daily per diem rate for a destination country from `validFrom`; `hr/business-trips/create` takes the latest rate valid on the trip's start date. Answers 409 when a rate for that country already starts on that date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.per_diem_rates_create(
    country_code="countryCode",
    daily_amount="121.00",
    valid_from=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**daily_amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**valid_from:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">per_diem_rates_list</a>(...) -> PerDiemRatesListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists per diem rates; filterable by `countryCode`, sortable by `countryCode` and `validFrom`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.per_diem_rates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[PerDiemRatesListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PerDiemRatesListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">per_diem_rates_delete</a>(...) -> PerDiemRatesDeleteHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a per diem rate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.per_diem_rates_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">business_trips_create</a>(...) -> BusinessTripsCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stores the trip as a draft with `days` counted as calendar days, both ends included, and `perDiemAmount` as the days times the company's rate for the destination valid on the start date (`hr/per-diem-rates/create`). Answers 422 when the trip ends before it starts or no rate covers the destination on that date, and 409 when the employee already has a trip overlapping the dates.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.business_trips_create(
    employee_id="employeeId",
    destination_country_code="destinationCountryCode",
    purpose="purpose",
    start_date=datetime.date.fromisoformat("2026-07-01"),
    end_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**destination_country_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**purpose:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**start_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">business_trips_get</a>(...) -> BusinessTripsGetHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads one business trip.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.business_trips_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">business_trips_list</a>(...) -> BusinessTripsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists business trips; filterable by `employeeId`, `status` and `payrollRunId`, sortable by `startDate`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.business_trips_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[BusinessTripsListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[BusinessTripsListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">business_trips_approve</a>(...) -> BusinessTripsApproveHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Sets the trip's status to `approved`. `payroll/runs/create` without explicit lines adds the per diem of every approved trip ending in the run month as an untaxed addition and sets the trip's `payrollRunId`; reversing or cancelling the run releases the trip again. Answers 409 when the trip is not a draft.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.business_trips_approve(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">business_trips_delete</a>(...) -> BusinessTripsDeleteHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a draft trip; answers 409 when the trip is not a draft.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.business_trips_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_records_create</a>(...) -> EmployeesRecordsCreateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Adds an education, qualification, certificate or training record to an employee, optionally linked to one of the company's uploaded files (`fileId`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_records_create(
    employee_id="employeeId",
    type="education",
    title="title",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `EmployeesRecordsCreateHrRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**title:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**institution:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_at:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_until:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**file_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_records_update</a>(...) -> EmployeesRecordsUpdateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes the given fields of an employee record; `issuedAt`, `validUntil` and `fileId` can be cleared with null.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_records_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[EmployeesRecordsUpdateHrRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**institution:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issued_at:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_until:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**file_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_records_delete</a>(...) -> EmployeesRecordsDeleteHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes an employee record.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_records_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_records_list</a>(...) -> EmployeesRecordsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists employee records; filterable by `employeeId`, `type` and `title`, sortable by `createdAt` and `issuedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_records_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[EmployeesRecordsListHrRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[EmployeesRecordsListHrRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">employees_attachments_list</a>(...) -> EmployeesAttachmentsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the files uploaded against an employee, newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.employees_attachments_list(
    employee_id="employeeId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">timesheets_generate</a>(...) -> TimesheetsGenerateHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the timesheet of the month for every employee with a contract in it, or for one employee with `employeeId`, replacing any existing timesheet: the Monday to Friday days within the contract get the contract's daily hours (its weekly hours over five), and for a Lithuanian company the public holidays are `holiday` days with 0 hours. Answers 422 when no contract covers the month.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.timesheets_generate(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**employee_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">timesheets_upsert</a>(...) -> TimesheetsUpsertHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates or replaces the timesheet of an employee for a month from the given days; `workedDays` and `workedHours` count the `work` and `business_trip` days with hours. Answers 422 for a day outside the month, a day given twice or more than 24 hours in a day. `payroll/runs/create` reads the timesheet for the paid days, the days worked and the business-trip days of the month.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.hr import TimesheetsUpsertHrRequestDaysItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.timesheets_upsert(
    employee_id="employeeId",
    year=1000000,
    month=1000000,
    days=[
        TimesheetsUpsertHrRequestDaysItem(
            day=1000000,
            hours="121.00",
            type="work",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**days:** `typing.List[TimesheetsUpsertHrRequestDaysItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">timesheets_get</a>(...) -> TimesheetsGetHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads the timesheet of an employee for a month.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.timesheets_get(
    employee_id="employeeId",
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">timesheets_list</a>(...) -> TimesheetsListHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the timesheets of a month, ordered by employee name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.timesheets_list(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">timesheets_delete</a>(...) -> TimesheetsDeleteHrResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a timesheet.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.timesheets_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## fleet
<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">vehicles_create</a>(...) -> VehiclesCreateFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a vehicle. The plate number is stored in upper case and must be unique in the company (409 otherwise); `fixedAssetId` must name an existing fixed asset. Uploaded `documents` are attached to the vehicle.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.vehicles_create(
    plate_number="plateNumber",
    make="make",
    model="model",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**plate_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**make:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**model:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**vin:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fuel_type:** `typing.Optional[VehiclesCreateFleetRequestFuelType]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**market_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_asset_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**technical_inspection_due:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**insurance_due:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[VehiclesCreateFleetRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">vehicles_update</a>(...) -> VehiclesUpdateFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a vehicle's details or set its `status` to `active`, `sold` or `scrapped`; omitted fields keep their value. A plate number already used by another vehicle is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.vehicles_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**plate_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**make:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**model:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**year:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**vin:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fuel_type:** `typing.Optional[VehiclesUpdateFleetRequestFuelType]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**market_value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_asset_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**technical_inspection_due:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**insurance_due:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[VehiclesUpdateFleetRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">vehicles_get</a>(...) -> VehiclesGetFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one vehicle with its current assignment, when an employee holds it today.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.vehicles_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">vehicles_list</a>(...) -> VehiclesListFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List vehicles with their current assignment. Filterable by `plateNumber`, `make`, `model` and `status`; sortable by `plateNumber`, `make` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.vehicles_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[VehiclesListFleetRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[VehiclesListFleetRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">assignments_create</a>(...) -> AssignmentsCreateFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Assign a vehicle to an employee from `fromDate`, open-ended or until `toDate`. A period that overlaps another assignment of the same vehicle is refused with 409, a `toDate` before `fromDate` with 422. `privateUse` makes the car a benefit in kind in `fleet/natura/preview`, and `employerPaysFuel` picks its rate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.assignments_create(
    vehicle_id="vehicleId",
    employee_id="employeeId",
    from_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**vehicle_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**private_use:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**employer_pays_fuel:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">assignments_end</a>(...) -> AssignmentsEndFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

End an open assignment on `toDate`. An assignment that already has an end date is refused with 409, a `toDate` before its `fromDate` with 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.assignments_end(
    id="id",
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">assignments_list</a>(...) -> AssignmentsListFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List vehicle assignments with the plate number and the employee's name. Filterable by `vehicleId`, `employeeId` and `privateUse`; sortable by `fromDate` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.assignments_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AssignmentsListFleetRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AssignmentsListFleetRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">natura_preview</a>(...) -> NaturaPreviewFleetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Preview the car benefit in kind of a month for a Lithuanian company: every assignment with `privateUse` that overlaps the month is valued at 0.75 % of the vehicle's market value when the employer pays the fuel, else 0.70 %, one row per employee and vehicle, with the total. A company registered in another country is refused with 422. The same amounts are added to a payroll run created with `includeNatura` (`payroll/runs/create`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.natura_preview(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## payroll
<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">departments_create</a>(...) -> DepartmentsCreatePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a department with a code and a name; answers 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.departments_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">departments_list</a>() -> DepartmentsListPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's departments ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.departments_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">schedules_create</a>(...) -> SchedulesCreatePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a work schedule with a code, a name and `hoursPerWeek` (default 40); answers 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.schedules_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**hours_per_week:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">schedules_list</a>() -> SchedulesListPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists the company's work schedules ordered by code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.schedules_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">payment_types_list</a>() -> PaymentTypesListPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads the payment types of the company country's payroll engine, each with the labels of the taxes, contributions and reporting lines it is subject to (`applies`), and the default type an untyped payment falls under. These codes are what `payroll/calc` and the additions of `payroll/runs/create` accept as `paymentType`. Answers 422 when Nordlet has no payroll engine for the company's country.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.payment_types_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">calc</a>(...) -> CalcPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Runs the company country's payroll engine once on a taxable base at a date, with the employee settings given in the body instead of an employee record, and returns the allowance, income tax, contributions, components and net; nothing is saved. `payments` passes typed payments to the engine; each `paymentType` must be a code from `payroll/payment-types/list` (422 otherwise). Answers 422 when Nordlet has no payroll engine for the company's country.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.calc(
    taxable_base="121.00",
    date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**taxable_base:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**apply_allowance:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**allowance_override:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pension_accumulation:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_term:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**benefit_in_kind:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**options:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**payments:** `typing.Optional[typing.List[CalcPayrollRequestPaymentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_create</a>(...) -> RunsCreatePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a draft payroll run for a month, computing each line with the company country's payroll engine, the employee's approved runs of the year so far and of the two previous years, the month's timesheet and `payDate` (default the last day of the month). Without `lines`, every active employee whose contract covers the month gets a line: the gross is the contract's monthly salary reduced to the paid working days of the contract and the timesheet, unless `grossOverrides` sets it; the per diems of approved business trips ending in the month are added untaxed and the trips linked to the run; for a Lithuanian company the car benefit in kind (`includeNatura`) and the compensation for unused leave of a contract ending in the month are added. With `lines`, only the given employees are computed with their gross, additions and deductions; a taxable addition may carry a `paymentType` from `payroll/payment-types/list` and `hours`. Answers 422 when the country has no engine, an employee is given twice, has two contracts in the month, has no contract and no gross, or is paid by the hour or day without a gross; 409 when a run for the month already exists or the accounting period is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_create(
    year=1000000,
    month=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**month:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**include_natura:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**gross_overrides:** `typing.Optional[typing.List[RunsCreatePayrollRequestGrossOverridesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[RunsCreatePayrollRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pay_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_get</a>(...) -> RunsGetPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads a payroll run with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_list</a>(...) -> RunsListPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists payroll runs without their lines; filterable by `status`, `year` and `month`, sortable by `createdAt`, `year` and `month`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RunsListPayrollRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RunsListPayrollRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">lines_attendance</a>(...) -> LinesAttendancePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The days and hours worked, the days on the register and the average hourly earnings that some countries report per employment. The Czech monthly employer report asks for all four. They can be set while the run is a draft.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.lines_attendance(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**days_worked:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**hours_worked:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**registered_days:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**average_hourly_earnings:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_approve</a>(...) -> RunsApprovePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Posts the run's journal entry dated the last day of the month and sets the status to `approved`: the wage expense (net pay, income tax, employee contributions and deductions) and the employer contributions are debited; the net payable, the income tax, the social contributions (on one account, or split between the employee and employer accounts when their codes differ) and the deductions are credited. The accounts default to the payroll accounts of the company's chart template; each can be given per call. Answers 409 when the run is not a draft or the accounting period is locked, 422 when the run has no lines or nothing to post, and emits `payroll_run.approved`. For an Irish company with the automation of the `ie-payroll-withholding` deadline switched on, the month's payroll submission is sent at once and a failure is added to the run's `warnings`. Undo with `payroll/runs/reverse`, pay with `payroll/payments/export`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_approve(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**wage_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**employer_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payable_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**gpm_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sodra_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**employer_social_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**deduction_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_reverse</a>(...) -> RunsReversePayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Posts a journal entry dated the last day of the month that mirrors the run's entry (debits and credits swapped), sets the status to `reversed` with the reason, and releases the business trips the run paid so the next run picks them up again. Answers 409 when the run is not approved, when part of it is matched to bank payments (`paidAmount`, unmatch them first) or when the accounting period is locked. Emits `payroll_run.reversed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_reverse(
    id="id",
    reason="reason",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">runs_cancel</a>(...) -> RunsCancelPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a draft run with its lines and releases the business trips linked to it; answers 409 when the run is not a draft. An approved run is undone with `payroll/runs/reverse`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.runs_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">payments_export</a>(...) -> PaymentsExportPayrollResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds a SEPA credit transfer file (pain.001.001.03) for an approved run: one transfer from the chosen bank account to each employee's IBAN for the line's net when it is positive, with a remittance text in `locale` (default the locale of the calling user) and the run period, executed on `executionDate` (default the company's current date). Answers 409 when the run is not approved, and 422 when the bank account has no IBAN or is not in the company's base currency, an employee has no IBAN (`hr/employees/update`) or no line has a positive net. The file is returned in `xml`; nothing is sent to the bank.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.payments_export(
    run_id="runId",
    bank_account_id="bankAccountId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**run_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**execution_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[PaymentsExportPayrollRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## agreements
<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">settings_get</a>() -> SettingsGetAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return whether automatic agreement billing is switched on for the company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">settings_update</a>(...) -> SettingsUpdateAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Switch automatic agreement billing on or off for the company. With it on, a scheduled job runs the same billing as `agreements/agreements/billing/run` for the company once a day.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.settings_update(
    auto_billing=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**auto_billing:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">types_create</a>(...) -> TypesCreateAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an agreement type with a `code` and a `name`. Answers 409 when the company already has a type with that code.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.types_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">types_list</a>(...) -> TypesListAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's agreement types. Filterable and sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.types_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[TypesListAgreementsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[TypesListAgreementsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_create</a>(...) -> AgreementsCreateAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an agreement for exactly one party, a partner, an employee or a bank account, which must exist in the company (400 otherwise). Without `kind`, an employee agreement is `employment`, a bank account agreement is `bank` and a partner agreement is `other`; a `documentRef` (the `storageKey` of an uploaded file) attaches that file to the agreement. Answers 409 when the company already has an agreement with that `number`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_create(
    number="number",
    start_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**start_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `typing.Optional[AgreementsCreateAgreementsRequestKind]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**employee_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_account_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_renew:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**billing_period:** `typing.Optional[AgreementsCreateAgreementsRequestBillingPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[AgreementsCreateAgreementsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.Optional[typing.List[AgreementsCreateAgreementsRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_get</a>(...) -> AgreementsGetAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one agreement with its items.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_update</a>(...) -> AgreementsUpdateAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the given fields of an agreement and return it with its items. The party, `number`, `startDate`, `currency` and items are not changed by this call.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `typing.Optional[AgreementsUpdateAgreementsRequestKind]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**auto_renew:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**value:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**billing_period:** `typing.Optional[AgreementsUpdateAgreementsRequestBillingPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[AgreementsUpdateAgreementsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_delete</a>(...) -> AgreementsDeleteAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark an agreement as deleted. It is no longer returned, changed or billed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_list</a>(...) -> AgreementsListAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's agreements without their items, each with `partnerName`. Filterable by `number`, `name`, `partnerId`, `employeeId`, `bankAccountId`, `kind`, `typeId`, `status`, `startDate`, `endDate` and `value`; sortable by `number`, `startDate` and `createdAt` (default `startDate` descending).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AgreementsListAgreementsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AgreementsListAgreementsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_generate_invoice</a>(...) -> AgreementsGenerateInvoiceAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft sale invoice for the next unbilled period of an active agreement that has a partner and a `billingPeriod`. The period follows the monthly, quarterly or annual grid from `startDate`, continues after the last period already invoiced for the agreement, and is prorated by days when it starts late or is cut by `endDate`; an `autoRenew` agreement has its `endDate` moved forward by whole terms instead (`renewedEndDate`). The lines come from the agreement items, else one line of `value`, with revenue recognised ratably over the period. Answers 422 when the agreement is not active, has no partner, billing period, items or value, carries VAT while the company is not a VAT payer, is fully billed through its end date, or when the next period starts after `asOfDate` (default today). Emits `agreement.invoice_generated`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_generate_invoice(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">agreements_billing_run</a>(...) -> AgreementsBillingRunAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate the invoices due up to `asOfDate` (default today) for every active agreement of the company that has a partner and a billing period, one invoice per period and at most 60 per agreement in one run, in the same way as `agreements/agreements/generate-invoice`. An agreement that is fully billed and whose `endDate` has passed is set to `expired`. A failing agreement is listed in `errors` and does not stop the run. Each invoice emits `agreement.invoice_generated`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.agreements_billing_run()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">insurance_policies_create</a>(...) -> InsurancePoliciesCreateAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an insurance policy. Answers 422 when `toDate` is before `fromDate`, 400 when `insurerPartnerId` is not a partner of the company, and 409 when the company already has a policy with that `policyNumber`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.insurance_policies_create(
    policy_number="policyNumber",
    insured_object="insuredObject",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**policy_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**insured_object:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**insurer_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**premium:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">insurance_policies_list</a>(...) -> InsurancePoliciesListAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's insurance policies. Filterable by `policyNumber`, `insurerPartnerId` and `toDate`; sortable by `policyNumber` and `toDate` (default `toDate` descending).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.insurance_policies_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[InsurancePoliciesListAgreementsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[InsurancePoliciesListAgreementsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">insurance_policies_delete</a>(...) -> InsurancePoliciesDeleteAgreementsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark an insurance policy as deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.insurance_policies_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## inventory
<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">settings_get</a>() -> SettingsGetInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the company's negative stock policy.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.settings_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">settings_update</a>(...) -> SettingsUpdateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the negative stock policy. With `reject` a consumption larger than the stock on hand of the item in the warehouse is refused with 422. With `allow` the missing quantity is written as a shortage priced at the unit cost of the last receipt in that warehouse (the item's purchase price when there is none); the next receipt of the item there settles the shortage and posts any cost difference between `inventory.cogs` and `inventory.stock`. A consumption from a named lot is refused with 422 under both policies.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.settings_update(
    negative_stock_policy="reject",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**negative_stock_policy:** `SettingsUpdateInventoryRequestNegativeStockPolicy` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">warehouses_create</a>(...) -> WarehousesCreateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a warehouse. 409 when the code already exists.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.warehouses_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**is_default:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">warehouses_list</a>(...) -> WarehousesListInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the warehouses. Filterable and sortable: code, name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.warehouses_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[WarehousesListInventoryRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[WarehousesListInventoryRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">warehouses_update</a>(...) -> WarehousesUpdateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the name or the country code of a warehouse.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.warehouses_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_receive</a>(...) -> StockReceiveInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a manual receipt of an item into a warehouse at `unitCost` (document type `manual_receipt`); the quantity must be positive (422). A lot- or serial-tracked item needs `lotNumber` (422); an unknown lot is created, and `expiryDate` is stored on a lot that has none. A serial-tracked item is received one unit at a time (422), and 409 when that serial number is already in stock. Open shortages of the item in the warehouse (negative stock policy `allow`) are settled from the receipt. Emits `stock.changed`. Receipts against a purchase order go through `purchases/receipts/create`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_receive(
    warehouse_id="warehouseId",
    item_id="itemId",
    date=datetime.date.fromisoformat("2026-07-01"),
    quantity="121.0000",
    unit_cost="121.000000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**unit_cost:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lot_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expiry_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_write_off</a>(...) -> StockWriteOffInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Consume a quantity of an item from a warehouse, oldest layers first (from one lot when `lotNumber` is given), and post a journal entry: debit the expense account (`expenseAccountCode`, default the chart's inventory expense account), credit the stock account each consumed layer was received on (the chart's inventory account for layers without one), or `inventoryAccountCode` for the whole cost when given. 409 when the accounting period of `date` is locked; 422 when the stock is insufficient under the `reject` policy or in the named lot. Emits `stock.changed` and, when the consumption takes the available quantity from above a reorder rule's minimum to at or below it, `stock.reorder_needed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_write_off(
    warehouse_id="warehouseId",
    item_id="itemId",
    date=datetime.date.fromisoformat("2026-07-01"),
    quantity="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lot_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**inventory_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_transfer</a>(...) -> StockTransferInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Move a quantity of an item from one warehouse to another: the source layers are consumed oldest first (from one lot when `lotNumber` is given) and received in the target with the same quantities, costs, lots and stock accounts (document type `warehouse_transfer`). 422 when both warehouses are the same or the source stock is insufficient under the `reject` policy. `inMovementId` is the first receipt when the consumption spans several lots or stock accounts. Emits `stock.changed` for both warehouses and `stock.reorder_needed` as `inventory/stock/write-off` does.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_transfer(
    from_warehouse_id="fromWarehouseId",
    to_warehouse_id="toWarehouseId",
    item_id="itemId",
    date=datetime.date.fromisoformat("2026-07-01"),
    quantity="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lot_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_take</a>(...) -> StockTakeInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Post a stock count for a warehouse. Each line names an item by `itemId` or `barcode` with its `countedQty`; the difference to the quantity on hand in the warehouse (all lots together) is written off oldest layers first or received as a surplus at `unitCost` (the item's purchase price when omitted; 422 when neither is set), with document type `stock_take`, and a surplus of a lot- or serial-tracked item needs `lotNumber` (422). The shortage cost less the surplus cost is posted in one journal entry between the expense account (`expenseAccountCode`, default the chart's inventory expense account) and the stock accounts (`inventoryAccountCode` for everything when given, else the accounts of the consumed layers and the chart's inventory account for the surpluses); nothing is posted and `journalTransactionId` is null when the net is zero. 409 when the accounting period of `date` is locked. Emits `stock.changed` per adjusted item.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.inventory import StockTakeInventoryRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_take(
    warehouse_id="warehouseId",
    date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        StockTakeInventoryRequestLinesItem(
            counted_qty="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[StockTakeInventoryRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**expense_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**inventory_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_levels</a>(...) -> StockLevelsInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the quantity and value on hand per item and warehouse, summed from the stock movements, optionally for one `warehouseId` and/or `itemId`. Rows with a zero quantity are left out.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_levels()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">stock_movements_list</a>(...) -> StockMovementsListInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the stock movements. Filterable: itemId, warehouseId, lotId, direction, documentType, date, quantity, totalCost. Sortable: date, createdAt, quantity, totalCost; default newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.stock_movements_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[StockMovementsListInventoryRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[StockMovementsListInventoryRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">lots_list</a>(...) -> LotsListInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the lots with their quantity on hand (the remaining quantity of the lot's incoming movements). Filterable: itemId, lotNumber, expiryDate. Sortable: lotNumber, expiryDate, createdAt; default newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.lots_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[LotsListInventoryRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[LotsListInventoryRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">lots_get</a>(...) -> LotsGetInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return a lot with its quantity on hand and its movements in date order.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.lots_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">lots_update</a>(...) -> LotsUpdateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the expiry date or the notes of a lot; null clears the value.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.lots_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**expiry_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">landed_costs_create</a>(...) -> LandedCostsCreateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Allocate an extra cost `amount` (positive, whole cents; 422 otherwise) over incoming stock movements, named by `movementIds` or taken from the lines of a goods receipt (`goodsReceiptId`; 422 when the receipt has no stock movements), in proportion to their cost (`by_value`) or quantity (`by_quantity`), largest remainder to the cent. The part of each share that belongs to the quantity still on hand raises the movement's remaining cost and recomputes its unit cost; the part that belongs to quantity already consumed is posted in a journal entry dated `date` debiting `inventory.cogs` and crediting the movement's stock account (`inventory.stock` when it has none), 409 when that period is locked. 422 when a movement is not incoming or the weights sum to zero. `sourceInvoiceId` records the purchase invoice the cost came from. Goods receipts come from `purchases/receipts/create`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.landed_costs_create(
    date=datetime.date.fromisoformat("2026-07-01"),
    amount="121.000000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**method:** `typing.Optional[LandedCostsCreateInventoryRequestMethod]` 
    
</dd>
</dl>

<dl>
<dd>

**goods_receipt_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**movement_ids:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**source_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">landed_costs_get</a>(...) -> LandedCostsGetInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return a landed cost with its allocation lines and the journal transaction it posted, if any.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.landed_costs_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">landed_costs_list</a>(...) -> LandedCostsListInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the landed costs without their lines. Filterable: date, method, goodsReceiptId, sourceInvoiceId. Sortable: date, createdAt, amount; default newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.landed_costs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[LandedCostsListInventoryRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[LandedCostsListInventoryRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">reorder_rules_create</a>(...) -> ReorderRulesCreateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a reorder rule for an item, for one warehouse or, without `warehouseId`, for the item over all warehouses; one rule per item and warehouse (409). While the rule is active, an outgoing movement or a reservation that takes the available quantity (on hand less reserved) from above `minQty` to at or below it emits `stock.reorder_needed` with the `reorderQty`. `inventory/reorder-rules/check` lists the rules currently at or below their minimum.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.reorder_rules_create(
    item_id="itemId",
    min_qty="121.0000",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**min_qty:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**reorder_qty:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">reorder_rules_update</a>(...) -> ReorderRulesUpdateInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the minimum quantity, the reorder quantity (null clears it), the active flag or the notes of a reorder rule.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.reorder_rules_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**min_qty:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**reorder_qty:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">reorder_rules_delete</a>(...) -> ReorderRulesDeleteInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a reorder rule.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.reorder_rules_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">reorder_rules_list</a>(...) -> ReorderRulesListInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the reorder rules. Filterable: itemId, warehouseId, isActive. Sortable: createdAt, minQty; default newest first.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.reorder_rules_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ReorderRulesListInventoryRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ReorderRulesListInventoryRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">reorder_rules_check</a>() -> ReorderRulesCheckInventoryResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the active reorder rules whose available quantity (on hand less reserved, in the rule's warehouse or over all warehouses) is at or below `minQty`, with the quantities. Emits no event.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.reorder_rules_check()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## production
<details><summary><code>client.production.<a href="src/nordlet/production/client.py">work_centers_create</a>(...) -> WorkCentersCreateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a work center with its `costPerHour`. `costAccountCode` must be a postable account of the chart (422 otherwise); when a production order completes, the labor cost of the operations run on this center is credited to it instead of the `production.laborApplied` posting rule account. A duplicate `code` is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.work_centers_create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**cost_per_hour:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**maintenance_interval_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">work_centers_update</a>(...) -> WorkCentersUpdateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a work center; only the fields sent are changed. `costAccountCode` must be a postable account of the chart (422 otherwise); a `code` already used by another work center is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.work_centers_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost_per_hour:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**maintenance_interval_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">work_centers_list</a>(...) -> WorkCentersListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List work centers. `nextMaintenanceDate` is the latest completed maintenance date (the creation date when there is none) plus `maintenanceIntervalDays`, null without an interval. Filterable by `code`, `name` and `isActive`; sortable by `code`, `name` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.work_centers_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[WorkCentersListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[WorkCentersListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">routings_create</a>(...) -> RoutingsCreateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a routing with its operations: `sequence`, work center, `setupMinutes`, `runMinutesPerUnit` and an optional `qualityCheckName` that becomes a pending quality check on every production order using the routing. Operation sequences must be unique (422); a duplicate `code` is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.production import RoutingsCreateProductionRequestOperationsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.routings_create(
    code="code",
    name="name",
    operations=[
        RoutingsCreateProductionRequestOperationsItem(
            sequence=1000000,
            name="name",
            work_center_id="workCenterId",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**operations:** `typing.List[RoutingsCreateProductionRequestOperationsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">routings_get</a>(...) -> RoutingsGetProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one routing with its operations in sequence order.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.routings_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">routings_list</a>(...) -> RoutingsListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List routings without their operations. Filterable by `code`, `name` and `isActive`; sortable by `code`, `name` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.routings_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[RoutingsListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[RoutingsListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">maintenance_create</a>(...) -> MaintenanceCreateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a `preventive` or `corrective` maintenance planned for a work center on `plannedDate`; it starts as `planned`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.maintenance_create(
    work_center_id="workCenterId",
    type="preventive",
    planned_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**work_center_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `MaintenanceCreateProductionRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**planned_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">maintenance_complete</a>(...) -> MaintenanceCompleteProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Mark a `planned` maintenance as completed on `completedDate`, with optional `downtimeHours` and `cost` (409 when it is already completed or cancelled). The work center's `nextMaintenanceDate` is then counted from the latest completed maintenance date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.maintenance_complete(
    id="id",
    completed_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**completed_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**downtime_hours:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cost:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">maintenance_cancel</a>(...) -> MaintenanceCancelProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel a `planned` maintenance (409 when it is already completed or cancelled).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.maintenance_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">maintenance_list</a>(...) -> MaintenanceListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List maintenance records. Filterable by `workCenterId`, `status` and `type`; sortable by `plannedDate` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.maintenance_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[MaintenanceListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[MaintenanceListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">boms_create</a>(...) -> BomsCreateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a bill of materials for a finished item. `outputQuantity` is the finished quantity made per unit of order quantity; each line's `quantity` is the component consumed per unit of order quantity, increased by its `scrapPercent` at completion; `routingId` is the default routing of assembly orders. A BOM that consumes its own finished item is refused with 422, a duplicate `code` with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.production import BomsCreateProductionRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.boms_create(
    code="code",
    name="name",
    finished_item_id="finishedItemId",
    lines=[
        BomsCreateProductionRequestLinesItem(
            component_item_id="componentItemId",
            quantity="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**finished_item_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[BomsCreateProductionRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**output_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**routing_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">boms_get</a>(...) -> BomsGetProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one bill of materials with its component lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.boms_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">boms_list</a>(...) -> BomsListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List bills of materials without their lines. Filterable by `code`, `name`, `finishedItemId` and `isActive`; sortable by `code` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.boms_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[BomsListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[BomsListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">orders_create</a>(...) -> OrdersCreateProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft production order for `quantity` units of a BOM in a warehouse; stock moves only at `production/orders/complete`. An `assembly` order takes its routing from `routingId`, else from the BOM, and copies the routing's operations onto the order (`plannedMinutes` = setup minutes + run minutes per unit × finished quantity, priced at the work center's current `costPerHour`) with a pending quality check for every operation that names one. A `routingId` on a `disassembly` order, an inactive routing or a routing without operations is refused with 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.orders_create(
    bom_id="bomId",
    warehouse_id="warehouseId",
    quantity="121.0000",
    date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bom_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[OrdersCreateProductionRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**routing_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">orders_record_operation</a>(...) -> OrdersRecordOperationProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record the `actualMinutes` spent on one operation of a draft production order; at completion the actual minutes, else the planned ones, price the operation's labor cost. Refused with 409 once the order is completed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.orders_record_operation(
    id="id",
    actual_minutes="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**actual_minutes:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">quality_checks_add</a>(...) -> QualityChecksAddProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Add a pending quality check to a draft production order (409 once the order is completed). The order cannot complete while a check is pending.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.quality_checks_add(
    order_id="orderId",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**order_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">quality_checks_record</a>(...) -> QualityChecksRecordProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record the result of a quality check as `passed` or `failed`, with the time and the actor (409 once the order is completed). Only a `pending` check blocks `production/orders/complete`; a `failed` one does not.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.quality_checks_record(
    id="id",
    result="passed",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**result:** `QualityChecksRecordProductionRequestResult` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">quality_checks_list</a>(...) -> QualityChecksListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List quality checks. Filterable by `orderId`, `result` and `name`; sortable by `createdAt` and `name`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.quality_checks_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[QualityChecksListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[QualityChecksListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">orders_complete</a>(...) -> OrdersCompleteProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Complete a draft production order on the order's date. An `assembly` consumes the components FIFO from the warehouse (line quantity × order quantity, increased by `scrapPercent`), prices each operation at its actual or planned minutes × `costPerHour`, receives the finished item at material cost + labor cost less the share of `scrappedQuantity`, and, when there is labor, scrap or a component stock account other than the finished one, posts a journal entry debiting the finished stock account (and the `production.scrap` rule account for the scrapped share) and crediting the component stock accounts and the work centers' cost accounts (or the `production.laborApplied` rule account); a `disassembly` consumes the finished item and receives the components at its cost shared by quantity. `componentsAccountCode` and `finishedAccountCode` default to the chart's production accounts. Refused with 409 when the order is already completed, a quality check is still pending or the accounting period is locked, and with 422 when the BOM has no lines, `scrappedQuantity` is given on a disassembly or exceeds the finished quantity, the assembly cost is zero, stock is insufficient, a received item needs lot or serial tracking, or a posting account is missing. Emits `stock.changed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.orders_complete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**scrapped_quantity:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**components_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**finished_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">orders_get</a>(...) -> OrdersGetProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one production order with its operations and quality checks.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.orders_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">orders_list</a>(...) -> OrdersListProductionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List production orders without operations and quality checks. Filterable by `bomId`, `warehouseId`, `status` and `type`; sortable by `date` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.orders_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[OrdersListProductionRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[OrdersListProductionRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ecommerce
<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_create</a>(...) -> OrdersCreateEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a sales order from an online channel in status `new`. The customer is `partnerId` or `partner` details: with an `email` the existing partner with that e-mail is reused, otherwise a new partner is created; without either the call is refused with 422. `currency` defaults to the company's invoice currency, and `shipToCountryCode` and `marketplace` are kept for the VAT treatment of the invoice at fulfilment. A second order with the same `channel` and `externalRef` is refused with 409. Emits `sales_order.created`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.ecommerce import OrdersCreateEcommerceRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_create(
    lines=[
        OrdersCreateEcommerceRequestLinesItem(
            description="description",
            quantity="121.0000",
            unit_price_excl_vat="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**lines:** `typing.List[OrdersCreateEcommerceRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**channel:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**external_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner:** `typing.Optional[OrdersCreateEcommerceRequestPartner]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**ship_to_country_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**marketplace:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_get</a>(...) -> OrdersGetEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one sales order with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_list</a>(...) -> OrdersListEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List sales orders without their lines. Filterable by `channel`, `externalRef`, `partnerId` and `status`; sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[OrdersListEcommerceRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[OrdersListEcommerceRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_reserve</a>(...) -> OrdersReserveEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reserve stock for a `new` order in `warehouseId` (default: the order's warehouse; 422 when neither is set). Each product line, and each product component of a set line, is checked against the warehouse's on-hand quantity less the existing reservations; when any item is short the call is refused with 422 and nothing is reserved. Otherwise a reservation is written per stock line, `stock.changed` (change type `reserve`) is emitted for each, and the order becomes `reserved`. An order in another status is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_reserve(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_fulfill</a>(...) -> OrdersFulfillEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Fulfil a `new` or `reserved` order: its reservations are released, the stock lines are consumed FIFO from the order's warehouse on `date` (default: the company's today), the cost of goods sold is posted as a journal entry debiting `cogsAccountCode` and crediting the stock accounts of the consumed layers (`inventoryAccountCode` when a layer has none), and a draft sale invoice for the order lines is created and linked as `invoiceId`, ready for `sales/invoices/issue`. With a `shipToCountryCode` on the order the invoice's VAT scheme is resolved for goods shipped there, as a marketplace sale when `marketplace` is set. Account codes default to the company's chart. Refused with 422 when the stock lines have no warehouse or stock is insufficient (unless the company allows negative stock), with 409 when the accounting period is locked or the order is already `fulfilled` or `cancelled`. Emits `sales_order.fulfilled` and `stock.changed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_fulfill(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**cogs_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**inventory_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">orders_cancel</a>(...) -> OrdersCancelEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel an order that is not fulfilled: its stock reservations are released, `stock.changed` (change type `release`) is emitted for each, and the status becomes `cancelled`. A fulfilled order is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.orders_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">products_list</a>(...) -> ProductsListEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's items as a shop catalogue, in order of last update, with price and stock. `price` is the item's price in `priceListId` when given, else its own sale price, and `currency` that of the price list, else the company's invoice currency; `vatRatePercent` falls back to the rate of the item's VAT classifier. For a product `onHand`, `reserved` and `available` are summed over all warehouses or over `warehouseId` only; for a set `available` is the number of sets its product components can still make; for a service they are null. With `updatedSince` only items changed after that time are returned, deleted ones included (`deleted: true`), so a shop can sync incrementally; without it only live items are listed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.products_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_list_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**updated_since:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">stock_list</a>(...) -> StockListEcommerceResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stock position per item and warehouse: `onHand`, `reserved` and their difference `available`, for all warehouses or `warehouseId` only. Only items with a positive quantity on hand are returned.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.stock_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## cash
<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">orders_create</a>(...) -> OrdersCreateCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a numbered cash receipt (series `KPO`) or cash disbursement (`KIO`) and posts it in the base currency between the cash account (`cashAccountCode`, default the cash account of the company's chart) and `counterAccountCode`; a receipt debits the cash account, a disbursement credits it. Linked to an invoice - `saleInvoiceId` for a receipt against an issued invoice or advance invoice or a disbursement against an issued credit note, `purchaseInvoiceId` for a disbursement against a registered purchase invoice - the counter account is the receivable or payable account of the posting rules, the invoice's paid amount and payment status (`partial` or `paid`) are updated, and `sale_invoice.paid` or `purchase_invoice.paid` is emitted when the invoice becomes fully paid. Answers 422 when both invoice ids are given, a receipt names a purchase invoice, `counterAccountCode` differs from the invoice's account, or the invoice is in another currency or belongs to another partner; 409 when `amount` exceeds the invoice's remaining amount or the accounting period of `date` is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.orders_create(
    type="receipt",
    date=datetime.date.fromisoformat("2026-07-01"),
    amount="121.0000",
    purpose="purpose",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `OrdersCreateCashRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**purpose:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**counter_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cash_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**employee_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">orders_get</a>(...) -> OrdersGetCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns one cash order.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.orders_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">orders_list</a>(...) -> OrdersListCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists cash orders. Filterable by `type`, `date`, `partnerId`, `employeeId`, `fullNumber` and `amount`; sortable by `date`, `fullNumber`, `createdAt` and `amount`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.orders_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[OrdersListCashRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[OrdersListCashRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">balance</a>(...) -> BalanceCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the balance of a cash account (default: the cash account of the company's chart) from the posted journal entries, up to and including `asOf` when given.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.balance()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cash_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**as_of:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">expense_reports_create</a>(...) -> ExpenseReportsCreateCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a numbered expense report (series `AA`) for the employee and posts it: each line's net amount is debited to its `accountCode` and the VAT total to the input VAT account of the posting rules (`purchases.vatReceivable`), or the gross amount to the line account when the company is not a VAT payer, and the total is credited to the cash advances account (`cash.advances`), which settles the employee's advance balance shown by `cash/advance-holders/balances`. Answers 422 when the total is zero or a line account is missing from the chart or not postable, and 409 when the accounting period of `date` is locked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.cash import ExpenseReportsCreateCashRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.expense_reports_create(
    employee_id="employeeId",
    date=datetime.date.fromisoformat("2026-07-01"),
    lines=[
        ExpenseReportsCreateCashRequestLinesItem(
            description="description",
            account_code="accountCode",
            net_amount="121.00",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**employee_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[ExpenseReportsCreateCashRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">expense_reports_get</a>(...) -> ExpenseReportsGetCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns one expense report with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.expense_reports_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">expense_reports_list</a>(...) -> ExpenseReportsListCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists expense reports without their lines. Filterable by `employeeId` and `date`; sortable by `date` and `number`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.expense_reports_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ExpenseReportsListCashRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ExpenseReportsListCashRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">advance_holders_balances</a>() -> AdvanceHoldersBalancesCashResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns, per employee, the cash advances issued to them (disbursements posted to the `cash.advances` account with the employee set), the amounts returned (receipts on the same account), the total settled by expense reports and the open balance (issued less returned less settled).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.advance_holders_balances()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## projects
<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">create</a>(...) -> CreateProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a project; `partnerId` is the customer that `projects/time-entries/bill` invoices by default. A duplicate `code` is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.create(
    code="code",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">update</a>(...) -> UpdateProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a project's name, customer, `status` (`active`, `completed`, `archived`) or notes; only the fields sent are changed. An archived project accepts no new time entries.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[UpdateProjectsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">get</a>(...) -> GetProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one project.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">list</a>(...) -> ListProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List projects. Filterable by `code`, `name`, `status` and `partnerId`; sortable by `code`, `name` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListProjectsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListProjectsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">time_entries_create</a>(...) -> TimeEntriesCreateProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record hours worked on a project on a date, optionally for an employee and with the `hourlyRate` used when billing. `hours` must be positive (422); an archived project is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.time_entries_create(
    project_id="projectId",
    date=datetime.date.fromisoformat("2026-07-01"),
    hours="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**project_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**hours:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**employee_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**billable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**hourly_rate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">time_entries_update</a>(...) -> TimeEntriesUpdateProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a time entry; only the fields sent are changed. `hours` must be positive (422); an entry already billed to an invoice cannot be changed (409).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.time_entries_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**hours:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**billable:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**hourly_rate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">time_entries_delete</a>(...) -> TimeEntriesDeleteProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a time entry (409 once it is billed).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.time_entries_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">time_entries_list</a>(...) -> TimeEntriesListProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List time entries. Filterable by `projectId`, `employeeId`, `billable`, `billedInvoiceId` and `date`; sortable by `date`, `createdAt` and `hours`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.time_entries_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[TimeEntriesListProjectsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[TimeEntriesListProjectsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">time_entries_bill</a>(...) -> TimeEntriesBillProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft sale invoice from the project's unbilled billable time entries, optionally limited to `dateFrom` and `dateTo`, and mark them billed; needs the `sales:write` scope, and the invoice is issued with `sales/invoices/issue`. The customer is `partnerId`, else the project's partner (422 without either); each entry is priced at its own `hourlyRate`, else the call's `hourlyRate` (422 when an entry has neither); `groupBy` `rate` makes one line per rate with the summed hours, `entry` one line per entry; `itemId`, `vatRatePercent` and `vatClassifierCode` go onto every line. No matching entries is 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.time_entries_bill(
    project_id="projectId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**project_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**hourly_rate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_classifier_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**group_by:** `typing.Optional[TimeEntriesBillProjectsRequestGroupBy]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">report</a>(...) -> ReportProjectsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Profitability per project: `revenue` and `costs` from posted journal entries tagged with the project (income accounts credit less debit, expense accounts debit less credit), `profit` as their difference, and the hours from time entries (total, billable, billed, unbilled, and the unbilled amount at the entries' hourly rates). `projectId` limits the report to one project; `dateFrom` and `dateTo` limit the journal dates and the entry dates. Nothing is changed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.report()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**project_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## transport
<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_create</a>(...) -> WaybillsCreateTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a draft waybill to the consignee. The cargo lines are `lines` or, when none are given and `saleInvoiceId` is set, the product lines of that sale invoice (422 when it has none); a line without `description`, `unit` or `productCode` takes them from its item. `documentDate` defaults to the company's today and `series` to `VAZ`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_create(
    consignee_partner_id="consigneePartnerId",
    dispatch_at=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    load_address="loadAddress",
    unload_address="unloadAddress",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**consignee_partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**dispatch_at:** `datetime.datetime` 
    
</dd>
</dl>

<dl>
<dd>

**load_address:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**unload_address:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**transporter_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**estimated_arrival_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**vehicle_plate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**trailer_plate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**driver_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**driver_surname:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**load_warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**value_eur:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[WaybillsCreateTransportRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_update</a>(...) -> WaybillsUpdateTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a draft waybill; omitted fields keep their value, the optional ones can be cleared with null, and `lines`, when given, replace all existing lines. A waybill that is already issued or cancelled is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**consignee_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**transporter_partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**dispatch_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**estimated_arrival_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**vehicle_plate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**trailer_plate:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**driver_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**driver_surname:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**load_warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**load_address:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**unload_address:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**value_eur:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**series:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.Optional[typing.List[WaybillsUpdateTransportRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_issue</a>(...) -> WaybillsIssueTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Issue a draft waybill: it takes the next number of its `series` for the year of `documentDate` and becomes `issued`. Without a vehicle plate or without lines the call is refused with 422, a waybill that is not a draft with 409. Only issued waybills can go into the Lithuanian i.VAZ file (`declarations/lt/ivaz/generate`) and the Romanian e-Transport declaration (`declarations/ro/etransport/build`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_issue(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_cancel</a>(...) -> WaybillsCancelTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel a draft or issued waybill. An already cancelled one is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_get</a>(...) -> WaybillsGetTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one waybill with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">waybills_list</a>(...) -> WaybillsListTransportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List waybills with the consignee's name. Filterable by `status`, `consigneePartnerId`, `documentDate`, `fullNumber` and `dispatchAt`; sortable by `createdAt`, `dispatchAt` and `fullNumber`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.waybills_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[WaybillsListTransportRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[WaybillsListTransportRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## pos
<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">devices_create</a>(...) -> DevicesCreatePosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a cash register (POS device). The serial number must be unique in the company; a repeat is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.devices_create(
    name="name",
    serial_number="serialNumber",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**serial_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**model:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">devices_update</a>(...) -> DevicesUpdatePosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a POS device's details or set `isActive`; an inactive device accepts no new shifts or reports. A serial number already used by another device is refused with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.devices_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**serial_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**model:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">devices_list</a>(...) -> DevicesListPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List POS devices. Filterable by `name` and `serialNumber`; sortable by `name`, `serialNumber` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.devices_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DevicesListPosRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DevicesListPosRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">reports_create</a>(...) -> ReportsCreatePosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a daily cash register report (Z-report) and post it to the ledger in one journal entry: the cash and card takings are debited to `cashAccountCode` and `cardAccountCode`, the net of the `vatLines` is credited to `revenueAccountCode` and their VAT to `vatAccountCode`. `itemLines` write the sold products off `warehouseId` FIFO (a set is expanded to its product components) and add the cost of goods sold, debited to `cogsAccountCode` against the stock accounts. Account codes default to the company's chart. Refused with 422 when cash plus card differs from the gross total, the item lines have no warehouse or the device is inactive, with 409 when the accounting period is locked or the `reportNumber` already exists. Emits `pos_report.created` and, per item line, `stock.changed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime
from nordlet.pos import ReportsCreatePosRequestVatLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.reports_create(
    report_number="reportNumber",
    date=datetime.date.fromisoformat("2026-07-01"),
    vat_lines=[
        ReportsCreatePosRequestVatLinesItem(
            vat_rate_percent="121.00",
            net_amount="121.0000",
            vat_amount="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**report_number:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**vat_lines:** `typing.List[ReportsCreatePosRequestVatLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**device_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cash_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**card_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**item_lines:** `typing.Optional[typing.List[ReportsCreatePosRequestItemLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**cash_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**card_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**revenue_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**cogs_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**inventory_account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">reports_get</a>(...) -> ReportsGetPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one POS report with its VAT lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.reports_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">reports_list</a>(...) -> ReportsListPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List POS reports without their VAT lines. Filterable by `date`, `reportNumber` and `deviceId`; sortable by `date`, `reportNumber` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.reports_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ReportsListPosRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ReportsListPosRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">shifts_open</a>(...) -> ShiftsOpenPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Open a shift on a POS device with the cash float `openingCash`. A device has at most one open shift (409 for a second); an inactive device is refused with 422. Give `warehouseId` when the shift will sell stock items; they are written off that warehouse when the shift is closed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.shifts_open(
    device_id="deviceId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**device_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**opening_cash:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">shifts_get</a>(...) -> ShiftsGetPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one POS shift.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.shifts_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">shifts_list</a>(...) -> ShiftsListPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List POS shifts. Filterable by `deviceId` and `status`; sortable by `openedAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.shifts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ShiftsListPosRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ShiftsListPosRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">receipts_create</a>(...) -> ReceiptsCreatePosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a receipt in an open shift, numbered per shift from 1. Each line's net, VAT and gross come from its VAT-inclusive unit price; a line without `description` takes its item's name. Refused with 422 when cash plus card differs from the receipt total or a stock item is sold in a shift opened without a warehouse, with 409 when the shift is closed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.pos import ReceiptsCreatePosRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.receipts_create(
    shift_id="shiftId",
    lines=[
        ReceiptsCreatePosRequestLinesItem(
            quantity="121.0000",
            unit_price_incl_vat="121.0000",
            vat_rate_percent="121.00",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**shift_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[ReceiptsCreatePosRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**cash_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**card_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">receipts_list</a>(...) -> ReceiptsListPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List receipts without their lines. Filterable by `shiftId`; sortable by `number` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.receipts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ReceiptsListPosRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ReceiptsListPosRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">receipts_get</a>(...) -> ReceiptsGetPosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one receipt with its lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.receipts_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">shifts_close</a>(...) -> ShiftsClosePosResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Close an open shift: its receipts are summed by VAT rate and by product into one POS report, created as by `pos/reports/create` with number `reportNumber` (default `Z-<device serial>-<n>`, n being the device's closed shifts plus one) on `date` (default: the company's today), which posts the takings and the stock write-off to the ledger and emits `pos_report.created`. The response adds `expectedCash` (opening cash plus the cash receipts) and `cashDifference` (`countedCash` less expected). A shift without receipts is refused with 422, a closed one with 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.shifts_close(
    id="id",
    counted_cash="121.00",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**counted_cash:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**report_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## calendar
<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">list</a>(...) -> ListCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Lists, in due-date order, the filing deadlines Nordlet derives for the company from its country and profile together with the company's own events, between `from` and `to` (default 45 days back to 120 days ahead of the company's current date). Each deadline carries its submissions, whether it can be filed with `calendar/submit`, amended, or built with `calendar/download`, and whether its automation is on; `includeDone: false` leaves out the rows that are completed, submitted or accepted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**include_done:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">get</a>(...) -> GetCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Reads one calendar row by `key`: the id of a company event, or `ruleKey:period` for a filing deadline with its submissions.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.get(
    key="key",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">submit</a>(...) -> SubmitCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

With amend: true the return is filed again as a correction of the one already submitted or accepted for the period; only returns whose format has a correction mark accept it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.submit(
    key="key",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**amend:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">download</a>(...) -> DownloadCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Builds the file of a deadline whose format Nordlet produces but whose administration takes it only through the company's own account or program. Nothing is sent and no filing is recorded.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.download(
    key="key",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">create</a>(...) -> CreateCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a company event (kind `custom`) with a title, a due date, notes and a done flag.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.create(
    title="title",
    due_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**title:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**done:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">update</a>(...) -> UpdateCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Changes a calendar row by `key`. A company event takes a new title, due date, notes or done flag; a filing deadline (`ruleKey:period`) takes only notes and done, keeps its own title and date, and gets a stored row the first time it is annotated.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.update(
    key="key",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**done:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">delete</a>(...) -> DeleteCalendarResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Deletes a company event by its id, or the stored notes and done mark of a filing deadline by `ruleKey:period`; the deadline itself still comes from the rules.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.delete(
    key="key",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## audit
<details><summary><code>client.audit.<a href="src/nordlet/audit/client.py">list</a>(...) -> ListAuditResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the audit log of the company: who did what to which entity, with the recorded change in `diff`. Filterable by `action`, `entity`, `entityId`, `actorType` and `actorId`; sortable by `createdAt` and `id`, newest first by default.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.audit.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListAuditRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListAuditRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## webhooks
<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">subscriptions_create</a>(...) -> SubscriptionsCreateWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Register a webhook endpoint for the given event types (`*` for every event). The URL must be an https address that resolves to a public network (422 otherwise). The signing secret is generated unless `secret` is given, and this call is the only one that returns it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.subscriptions_create(
    url="url",
    events=[
        "agreement.invoice_generated"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**url:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.List[SubscriptionsCreateWebhooksRequestEventsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**secret:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">subscriptions_list</a>(...) -> SubscriptionsListWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's webhook subscriptions with their last delivery state. Filterable by `url` and `isActive`; sortable by `createdAt` and `url`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.subscriptions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SubscriptionsListWebhooksRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SubscriptionsListWebhooksRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">subscriptions_update</a>(...) -> SubscriptionsUpdateWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the URL, event types or `isActive` flag of a subscription; at least one field is required (400) and a new URL must be an https address that resolves to a public network (422). Setting `isActive` to true also clears `pausedAt` and `consecutiveFailures`, which is how a subscription paused after 5 failed deliveries in a row is switched back on.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.subscriptions_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**events:** `typing.Optional[typing.List[SubscriptionsUpdateWebhooksRequestEventsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">subscriptions_delete</a>(...) -> SubscriptionsDeleteWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a webhook subscription.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.subscriptions_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">deliveries_list</a>(...) -> DeliveriesListWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's webhook deliveries, newest first. Filterable by `status`, `eventType` and `subscriptionId`; sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.deliveries_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DeliveriesListWebhooksRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DeliveriesListWebhooksRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">deliveries_redeliver</a>(...) -> DeliveriesRedeliverWebhooksResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send a delivery again now: its status goes back to `pending` with the attempt count and last error cleared. Answers 409 when the subscription is inactive.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.deliveries_redeliver(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## bank
<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">accounts_create</a>(...) -> AccountsCreateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a bank, Stripe or broker account. `currency` defaults to the company base currency and `accountCode` to the default bank account of the chart of accounts. A `documentRef` also creates a bank agreement with that document attached. A Stripe account with an `iban` is refused with 422; an account with the same IBAN already existing answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.accounts_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[AccountsCreateBankRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**document_ref:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">accounts_list</a>(...) -> AccountsListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the bank accounts of the company. Filterable by name, type, iban and isActive; sortable by name and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.accounts_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[AccountsListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[AccountsListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">accounts_update</a>(...) -> AccountsUpdateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the name, type, IBAN, ledger account code or active flag of a bank account. Setting type to stripe clears the IBAN, and sending an `iban` together with it is refused with 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.accounts_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[AccountsUpdateBankRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**account_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_import</a>(...) -> TransactionsImportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Insert statement lines (up to 1000 per call) into a bank account as new transactions. A line without `currency` takes the account currency; a line in another currency is refused with 422. A line whose `externalId` is already on the account is skipped and counted in `skipped`. An incoming line that an active match rule (`bank/match-rules/create`) recognises is linked to its settlement batch.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.bank import TransactionsImportBankRequestTransactionsItem
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_import(
    bank_account_id="bankAccountId",
    transactions=[
        TransactionsImportBankRequestTransactionsItem(
            date=datetime.date.fromisoformat("2026-07-01"),
            amount="-121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**transactions:** `typing.List[TransactionsImportBankRequestTransactionsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">statements_import</a>(...) -> StatementsImportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Import a statement file into a bank account: camt.053 XML, MT940, a Stripe balance CSV or a Revolut Business CSV, chosen by `format` or by the type of `templateId` (an iso20022 template also takes MT940 content). Statements whose IBAN or currency differ from the account are left out; the call is refused with 422 when none remains, when a line is in another currency, when the file lacks the columns or elements the template requires or when it holds more than 50000 lines. Lines already on the account are skipped, and Stripe movements already posted through a settlement payout are skipped with a warning. With a template, the mapped fields are posted to their ledger accounts, partners are created, payments are matched to the invoices they reference, and invoices, credit notes or advance invoices are issued where the template asks for them (`invoiceMetaField`, `advanceInvoices`); `transfersCsv` posts the lender payouts and commissions of a Stripe template. Invoices issued this way are announced as `sale_invoice.issued`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.statements_import(
    bank_account_id="bankAccountId",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**template_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**format:** `typing.Optional[StatementsImportBankRequestFormat]` 
    
</dd>
</dl>

<dl>
<dd>

**transfers_csv:** `typing.Optional[str]` — Stripe transfers export (plain CSV or base64) used to post lender payouts and commissions
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_list</a>(...) -> TransactionsListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the bank transactions of the company. Filterable by id, bankAccountId, status, matchedDocumentId, date, amount, counterpartyIban, counterpartyName and externalId; sortable by date, createdAt and amount.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[TransactionsListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[TransactionsListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_match</a>(...) -> TransactionsMatchBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Match one new bank transaction to a document: an issued sale invoice or advance for incoming money; an issued sale credit note, a registered purchase invoice or an approved payroll run (company currency only) for outgoing money. Posts the payment journal transaction between the bank account and the receivable, payable or net payable account, with any exchange difference on the gain or loss account, raises the paid amount of the document and sets the line to matched. `invoiceAmount` states the amount settled on an invoice in another currency; in the same currency it must equal the payment (422). Answers 409 when the line is already matched, when the amount exceeds the remaining balance of the document or when the accounting period of the line date is locked. A document that becomes fully paid is announced as `sale_invoice.paid` or `purchase_invoice.paid`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_match(
    transaction_id="transactionId",
    document_type="sale_invoice",
    document_id="documentId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**transaction_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `TransactionsMatchBankRequestDocumentType` 
    
</dd>
</dl>

<dl>
<dd>

**document_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_match_many</a>(...) -> TransactionsMatchManyBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The documents are issued sale invoices or advances for incoming money; issued sale credit notes, registered purchase invoices or approved payroll runs for outgoing money. Each must be in the currency of the payment, each allocation must be above zero, a document may appear once and the allocations must add up to the payment (422 otherwise). One journal transaction carries the bank entry, one entry per document and any exchange difference; the line is matched as an `invoice_allocation`. Answers 409 when the line is already matched, when an allocation exceeds the remaining balance of its document or when the accounting period of the line date is locked. Each document that becomes fully paid is announced as `sale_invoice.paid` or `purchase_invoice.paid`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.bank import TransactionsMatchManyBankRequestAllocationsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_match_many(
    transaction_id="transactionId",
    allocations=[
        TransactionsMatchManyBankRequestAllocationsItem(
            document_type="sale_invoice",
            document_id="documentId",
            amount="121.0000",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**transaction_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**allocations:** `typing.List[TransactionsMatchManyBankRequestAllocationsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_unmatch</a>(...) -> TransactionsUnmatchBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Undo a match. A payment matched to an invoice, or a line posted by an import template, gets a reversing journal transaction dated date (default: today) and the invoice paid amount and payment status are restored; a line linked to a payment-provider settlement is only unlinked. The line returns to status new.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_unmatch(
    transaction_id="transactionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**transaction_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_record</a>(...) -> TransactionsRecordBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a payment that is on no imported statement: inserts a bank transaction on the account dated `date` (positive for a sale invoice, negative for a purchase invoice or payroll run, in the account currency) and matches it to the document with the checks, posting and `sale_invoice.paid` or `purchase_invoice.paid` event of `bank/transactions/match`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_record(
    bank_account_id="bankAccountId",
    date=datetime.date.fromisoformat("2026-07-01"),
    amount="121.0000",
    document_type="sale_invoice",
    document_id="documentId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `TransactionsRecordBankRequestDocumentType` 
    
</dd>
</dl>

<dl>
<dd>

**document_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">payments_export</a>(...) -> PaymentsExportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build a SEPA credit transfer file (pain.001.001.03) that pays the remaining amount of each registered purchase invoice from the bank account on `executionDate` (default: today), to the partner's default bank account. The bank account needs an IBAN and every invoice must be in EUR and have a partner bank account on file (422 otherwise, see `partners/bank-accounts/create`); an invoice that is already paid answers 409. The file is returned as `xml`; nothing is posted or marked paid.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.payments_export(
    bank_account_id="bankAccountId",
    purchase_invoice_ids=[
        "purchaseInvoiceIds"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**purchase_invoice_ids:** `typing.List[str]` 
    
</dd>
</dl>

<dl>
<dd>

**execution_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_create</a>(...) -> ImportTemplatesCreateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

A template of type stripe, iso20022, revolut or bank_connection names the fields of the file or feed: a field with an `accountCode` is posted to that ledger account on import, a field with `createPartner` creates the customer, supplier or fee partner. `invoiceMetaField` is the Stripe metadata key (stripe) or the reference field (other types) by which payments are linked to invoices; with it `invoiceVatRatePercent`, `invoiceItemId` and, outside Stripe, `advanceInvoices` apply. `companyMetaField`, `lenderMetaField`, the operation types and the refund labels are for Stripe templates only. A template with the same name already existing answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_create(
    name="name",
    type="stripe",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `ImportTemplatesCreateBankRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**fields:** `typing.Optional[typing.List[ImportTemplatesCreateBankRequestFieldsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**meta_fields:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**company_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**advance_invoices:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**authorization_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payout_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**commission_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lender_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partial_refund_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**full_refund_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_update</a>(...) -> ImportTemplatesUpdateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a company import template under the rules of `bank/import-templates/create`; a change of `type` re-checks the existing fields against the new type. Built-in templates cannot be changed. A name already used by another template answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ImportTemplatesUpdateBankRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**fields:** `typing.Optional[typing.List[ImportTemplatesUpdateBankRequestFieldsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**meta_fields:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_vat_rate_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**company_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**advance_invoices:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**authorization_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payout_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**commission_operation_type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**lender_meta_field:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**partial_refund_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**full_refund_label:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_delete</a>(...) -> ImportTemplatesDeleteBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a company import template. Built-in templates cannot be deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_get</a>(...) -> ImportTemplatesGetBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one import template, a company one or a built-in one.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_list_builtin</a>() -> ImportTemplatesListBuiltinBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Today the Revolut Business template: the Revolut CSV fields, with fees, card payments and top-ups posted to the accounts of the posting rules, the sender and beneficiary names creating partners and the Reference column linking payments to invoices. The rows carry `builtin: true`, are readable with `bank/import-templates/get` and are not in `bank/import-templates/list`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_list_builtin()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_list</a>(...) -> ImportTemplatesListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the import templates of the company (the built-in ones are under `bank/import-templates/list-builtin`). Filterable by name and type; sortable by name and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.import_templates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ImportTemplatesListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ImportTemplatesListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">match_rules_create</a>(...) -> MatchRulesCreateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a rule that links incoming bank lines to the settlement batches of a payment provider when lines are imported and when a batch is posted. A line whose description, counterparty name or external id contains `pattern` (case-insensitive) is linked to the open batch of `provider` whose payout id follows `payoutIdPrefix` in the line text or, without a prefix, to the single open batch on the same bank account with the same currency and net amount and a payout date within `dateWindowDays` of the line date. `bankAccountId` limits the rule to one account.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.match_rules_create(
    name="name",
    pattern="pattern",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**pattern:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**provider:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payout_id_prefix:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_account_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_window_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">match_rules_update</a>(...) -> MatchRulesUpdateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change a match rule; `payoutIdPrefix` and `bankAccountId` are cleared with null.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.match_rules_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**provider:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pattern:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**payout_id_prefix:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_account_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_window_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**is_active:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">match_rules_delete</a>(...) -> MatchRulesDeleteBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a match rule.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.match_rules_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">match_rules_list</a>() -> MatchRulesListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the match rules of the company, ordered by name.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.match_rules_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">mandates_create</a>(...) -> MandatesCreateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record a SEPA direct debit mandate a partner has signed: debtor IBAN and BIC, scheme (CORE or B2B), recurrent or one-off, and the signature date. `reference` is the mandate reference written into the collection files; without one `MNDT-` followed by a generated id is used. `debtorName` defaults to the partner name. A reference already in use answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.mandates_create(
    partner_id="partnerId",
    iban="iban",
    signature_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**signature_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**scheme:** `typing.Optional[MandatesCreateBankRequestScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**sequence_type:** `typing.Optional[MandatesCreateBankRequestSequenceType]` 
    
</dd>
</dl>

<dl>
<dd>

**reference:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**debtor_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">mandates_update</a>(...) -> MandatesUpdateBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the BIC, debtor name or notes of a mandate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.mandates_update(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**debtor_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">mandates_cancel</a>(...) -> MandatesCancelBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cancel an active mandate. A mandate that is already cancelled or completed answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.mandates_cancel(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">mandates_get</a>(...) -> MandatesGetBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one mandate. `expiresOn` is 36 months after the last collection, or after the signature date when nothing has been collected.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.mandates_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">mandates_list</a>(...) -> MandatesListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the mandates of the company. Filterable by partnerId, status, scheme, reference and iban; sortable by createdAt and signatureDate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.mandates_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[MandatesListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[MandatesListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">direct_debits_candidates</a>(...) -> DirectDebitsCandidatesBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the issued EUR sale invoices that are unpaid or partly paid and whose partner holds an active mandate, each with the mandate `bank/direct-debits/export` would use (the most recently signed active one). Filterable by partnerId, fullNumber, issueDate and dueDate; sortable by issueDate, dueDate, fullNumber, grossTotal and createdAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.direct_debits_candidates()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[DirectDebitsCandidatesBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[DirectDebitsCandidatesBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">direct_debits_export</a>(...) -> DirectDebitsExportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build a SEPA direct debit file (pain.008.001.02) that collects the remaining amount of each issued EUR sale invoice into the bank account on `collectionDate` (default: today) under the partner's most recently signed active mandate. The bank account needs an IBAN and the company a valid `sepaCreditorId` (422, see `account/companies/update`); an invoice whose partner has no active mandate, or whose mandate expired (36 months without a collection), answers 422; an invoice already paid, or a one-off mandate asked to collect more than one invoice, answers 409. The sequence type is OOFF for a one-off mandate, FRST for the first collection under a recurrent one and RCUR after that. On success the collection count and last collection date of each mandate are advanced and a one-off mandate is completed; nothing is posted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.direct_debits_export(
    bank_account_id="bankAccountId",
    sale_invoice_ids=[
        "saleInvoiceIds"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**sale_invoice_ids:** `typing.List[str]` 
    
</dd>
</dl>

<dl>
<dd>

**collection_date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">transactions_suggest_matches</a>(...) -> TransactionsSuggestMatchesBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Suggest documents for a new bank transaction: issued sale invoices and advances for incoming money; registered purchase invoices, issued sale credit notes and approved payroll runs for outgoing money. Candidates are unpaid documents whose remaining balance covers the payment (any balance when in another currency), scored by an equal remaining balance, the document number or payroll period in the payment description and a counterparty IBAN or name matching the partner or an employee on the run; the best `limit` come back with their reasons. A transaction that is already matched answers 409.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.transactions_suggest_matches(
    transaction_id="transactionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**transaction_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_import</a>(...) -> SettlementsImportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Import a Stripe payout report into settlement batches, one per payout: the itemized payout reconciliation CSV (`format` payout_reconciliation) or the unified payments export with its Transfer column (unified_payments); another CSV is refused with 422. Rows without a payout, the payout rows themselves and unsettled payments are skipped and counted. Each line is matched to an issued sale invoice through the references the report carries (the external reference of a sales order or an invoice number) or through a charge matched earlier. A payout already imported receives its new lines while the batch is in status imported and is skipped once posted; a payout mixing currencies answers 422. Emits `settlement.imported` for a new batch and `settlement.updated` for one that received lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_import(
    bank_account_id="bankAccountId",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**provider:** `typing.Optional[SettlementsImportBankRequestProvider]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_list</a>(...) -> SettlementsListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the settlement batches with their line counts and the clearing figures against the bank lines. Filterable by provider, payoutId, status, currency and bankAccountId; sortable by payoutDate, createdAt and netTotal.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SettlementsListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SettlementsListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_get</a>(...) -> SettlementsGetBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one settlement batch with its lines, each with the invoice it is matched to and the bank line that cleared it (`clearingBooked`, `clearingDifference`, `clearingUnposted`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_match</a>(...) -> SettlementsMatchBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Match a settlement line to an issued sale invoice or advance by hand (`matchStatus` manual), or clear the match with `invoiceId` null. Only lines of the categories charge, refund, dispute, dispute_reversal and partial_capture_reversal can be matched (422), and only while the batch is in status imported (409).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_match(
    line_id="lineId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**line_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_commission</a>(...) -> SettlementsCommissionBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

A line with its own rate or amount is split with that value when the batch is posted. A line without one falls back to the commissionPercent given to the posting call, and without that the amount goes to the suspense account. Send both fields as null to clear the line back to the fallback.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_commission(
    line_id="lineId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**line_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**commission_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**commission_amount:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_link</a>(...) -> SettlementsLinkBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Attach the incoming bank-statement line that carries this payout to the settlement batch.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_link(
    id="id",
    bank_transaction_id="bankTransactionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bank_transaction_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_unlink</a>(...) -> SettlementsUnlinkBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Detach the bank-statement line from the settlement batch and return the line to unmatched.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_unlink(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">settlements_post</a>(...) -> SettlementsPostBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Post a settlement batch dated `date` (default: the payout date, else today): the bank account receives the net payout, the matched sale invoices are settled against the receivable (the receivable of each partner in a journal transaction of its own when invoices of several partners are settled), the provider fees, the marketplace commission and the seller payable are booked, and a payout in another currency is converted at the rate of that date with the exchange difference against each invoice's own rate on the gain or loss account. A line without a matched invoice is split by its own rate or amount, else by `commissionPercent`, else parked on the suspense account; a line already imported as a movement of a bank account is posted against that account instead. Answers 409 when the batch is already posted or the period is locked, 422 when it has no lines. The payout is linked to the bank line a match rule recognises. Emits `settlement.posted`, `sale_invoice.paid` for each invoice that becomes paid and `refund_liability.actual` for refunds of invoices carrying a refund liability.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.settlements_post(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**commission_percent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">securities_import</a>(...) -> SecuritiesImportBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Import an Interactive Brokers activity statement (CSV) into a bank account of type `broker`; refused with 422 for another account type, a file that is not an IBKR statement, a statement of a different IBKR account than the bank account already holds, or a trade older than the latest trade already imported (statements go in in date order). Rows already imported are skipped. Dividends, withholding tax, interest and fees are posted against the broker account; stock, option and futures trades are matched FIFO against the open lots and post the cost to `securities.investments` and the realised result to `securities.gain` or `securities.loss` (posting rules), one journal entry per date in the base currency at the rate of the day (422 without a rate, 409 when the date's period is locked). Deposits, corporate actions and currency conversions are stored as `not_posted` with a note.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.securities_import(
    bank_account_id="bankAccountId",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**bank_account_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**file_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">securities_list</a>(...) -> SecuritiesListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the securities imports, newest first; filterable by `bankAccountId` and `brokerAccount`, sortable by `createdAt` and `realizedTotal`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.securities_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SecuritiesListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SecuritiesListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">securities_get</a>(...) -> SecuritiesGetBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one securities import with its operations in date order, each with its posting status, its amounts in the base currency and the journal transaction it was posted in.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.securities_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">securities_operations_list</a>(...) -> SecuritiesOperationsListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the imported securities operations, newest first; filterable by `bankAccountId`, `kind`, `status`, `symbol` and `date`, sortable by `date` and `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.securities_operations_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[SecuritiesOperationsListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[SecuritiesOperationsListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_banks_list</a>(...) -> FeedsBanksListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read from the bank-feed provider configured on the API server or in platform settings (Enable Banking or an HTTP bridge, named in `provider`), for one `country` or all. Without a provider the call answers 503.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_banks_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**country:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_connections_start</a>(...) -> FeedsConnectionsStartBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a pending bank connection and asks the provider for the authorization page of the bank. `url` is where the user authorizes access for `validForDays` (default 90); `reference` is the state the bank sends back and what `bank/feeds/connections/complete` takes. `redirectUrl` falls back to the one in platform settings, and the call is refused with 422 when neither is set.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_connections_start(
    aspsp_name="aspspName",
    aspsp_country="aspspCountry",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**aspsp_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**aspsp_country:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**psu_type:** `typing.Optional[FeedsConnectionsStartBankRequestPsuType]` 
    
</dd>
</dl>

<dl>
<dd>

**redirect_url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_for_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**language:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_connections_complete</a>(...) -> FeedsConnectionsCompleteBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Exchanges `code` for a provider session, sets the connection to active with the consent expiry the bank reports, and records every account of the session as a bank-feed account, not yet linked to a ledger account (`bank/feeds/accounts/link`). A connection that is already active answers 409. When the provider refuses the code the connection goes to status error with the message in `error`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_connections_complete(
    reference="reference",
    code="code",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**reference:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_connections_get</a>(...) -> FeedsConnectionsGetBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read one bank connection with its bank-feed accounts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_connections_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_connections_list</a>(...) -> FeedsConnectionsListBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the bank connections of the company, without their accounts. Filterable by status, provider and aspspCountry; sortable by createdAt and lastSyncedAt.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_connections_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[FeedsConnectionsListBankRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[FeedsConnectionsListBankRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_connections_delete</a>(...) -> FeedsConnectionsDeleteBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Closes the provider session when the connection has one and a provider is configured (a failure at the bank does not stop the call), then deletes the connection and its bank-feed accounts. The ledger bank accounts and the transactions already imported stay.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_connections_delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_accounts_link</a>(...) -> FeedsAccountsLinkBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Give exactly one of `bankAccountId` (an existing ledger bank account) or `createBankAccount` (a new one with the IBAN and currency of the feed account; `accountCode` defaults to the default bank account of the chart of accounts). `syncFrom` is the date the first sync starts from; without it the first sync covers the last 90 days.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_accounts_link(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bank_account_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**create_bank_account:** `typing.Optional[FeedsAccountsLinkBankRequestCreateBankAccount]` 
    
</dd>
</dl>

<dl>
<dd>

**sync_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_accounts_configure</a>(...) -> FeedsAccountsConfigureBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

`importTemplateId` must be a template of type bank_connection, or null to apply none. `syncSchedule` is manual, daily, weekly or monthly; every account whose schedule is not manual is synced by Nordlet when it is due. At least one of the two must be given.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_accounts_configure(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**import_template_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sync_schedule:** `typing.Optional[FeedsAccountsConfigureBankRequestSyncSchedule]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_sync</a>(...) -> FeedsSyncBankResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Fetches the transactions of every linked bank-feed account of the connection, or of `feedAccountId` alone, from `dateFrom` (default: seven days before the last sync, else the `syncFrom` of the account, else 90 days back) to `dateTo`, and inserts the new ones into the linked ledger bank account; lines already there count as `skipped`. An import template set on the account is applied as in `bank/statements/import`. Answers 409 when the connection is not active or has no session, and when the bank returns more than 20 pages for the range (keep `dateFrom` and set an earlier `dateTo`). A provider failure is written to the `error` of the connection, and one that is not retryable sets its status to error. The outcome is announced as `bank_feed.synced`, and invoices the template issues as `sale_invoice.issued`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.feeds_sync(
    connection_id="connectionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**connection_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**feed_account_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_from:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## files
<details><summary><code>client.files.<a href="src/nordlet/files/client.py">upload</a>(...) -> UploadFilesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Store a base64-encoded file of up to 10 MB (413 above that) under an `entity` and optional `entityId`, and return its record with the SHA-256 of the content and its `storageKey`, which other calls take as `documentRef`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.upload(
    entity="entity",
    file_name="fileName",
    mime_type="mimeType",
    content="content",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**entity:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**file_name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**mime_type:** `str` — Stored as the bare media type; only PNG, JPEG, GIF, WebP and PDF files are shown in the browser, every other type is downloaded
    
</dd>
</dl>

<dl>
<dd>

**content:** `str` — Base64-encoded file content
    
</dd>
</dl>

<dl>
<dd>

**entity_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">get</a>(...) -> GetFilesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return a file record with its content, base64-encoded.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">list</a>(...) -> ListFilesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's files. Filterable by `entity`, `entityId` and `fileName`; sortable by `createdAt`, `fileName` and `sizeBytes`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[ListFilesRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[ListFilesRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">delete</a>(...) -> DeleteFilesResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a file record and its stored content.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.delete(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## reports
<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">trial_balance</a>(...) -> TrialBalanceReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Trial balance of the posted ledger for a period: for every account with an opening balance or movement, the balance before `fromDate`, the debit and credit turnover between `fromDate` and `toDate`, and the closing balance, with debit and credit totals. Template account names follow the `Accept-Language` header.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.trial_balance(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">size_category</a>(...) -> SizeCategoryReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Classify the company's size for a calendar year as micro, small, medium or large from total assets at the year end, the net turnover of the year and the average number of employees under employment contracts, against the limits returned in `thresholds`; a category applies when at least two of its three limits are met. This is the default category of `reports/financial-statements`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.size_category(
    year=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**year:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">financial_statements</a>(...) -> FinancialStatementsReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Balance sheet at `toDate` and profit and loss for the period from the posted ledger, year-end closing entries excluded, laid out by size category: `category` when given, else the one `reports/size-category` derives for the period. Micro gets the short balance sheet and profit and loss; the other categories add the balance sheet and profit and loss detail; medium and large also get the changes in equity and a cash flow summary. Line groupings follow the company's chart template.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.financial_statements(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[FinancialStatementsReportsRequestCategory]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">general_journal</a>(...) -> GeneralJournalReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Posted journal transactions of a period in date order, each with its lines (account, debit, credit), paged with `page` and `pageSize` and the total count. Template account names follow the `Accept-Language` header.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.general_journal(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">gl_detail</a>(...) -> GlDetailReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Ledger card of one account for a period: the opening balance before `fromDate`, every posted line in date order with a running balance, and the closing balance.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.gl_detail(
    account_code="accountCode",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**account_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">partner_balances</a>() -> PartnerBalancesReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Open balance per partner: receivables from issued sale invoices and payables from registered purchase invoices that are not fully paid, credit notes reducing the balance, converted to the base currency at the document rate, with totals.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.partner_balances()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">debt_aging</a>(...) -> DebtAgingReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Ageing of the open receivables or payables (`side`) at `asOf` (default the company's current date) per partner: not yet due, 1 to 30, 31 to 60, 61 to 90 and over 90 days past the due date. Counts documents dated on or before `asOf` and payments made up to that date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.debt_aging()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**side:** `typing.Optional[DebtAgingReportsRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**as_of:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">monthly_summary</a>(...) -> MonthlySummaryReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

One row per calendar month for the last `months` months ending with the current one: the receivable and payable balances at the end of the month and the revenue, expenses and net result posted in it, year-end closing entries excluded.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.monthly_summary()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**months:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">stock_balance</a>(...) -> StockBalanceReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Quantity and value on hand per item and warehouse at `asOf`, summed from the stock movements dated on or before it; `warehouseId` limits the report to one warehouse. Rows with zero quantity and zero value are left out.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.stock_balance(
    as_of=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">stock_movement</a>(...) -> StockMovementReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stock movement per item for a period: opening quantity and value before `fromDate`, quantities and values received and issued between `fromDate` and `toDate`, and the closing figures; `warehouseId` and `itemId` narrow the report.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.stock_movement(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**item_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">vat_summary</a>(...) -> VatSummaryReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

VAT of issued sale invoices (by issue date) or registered purchase invoices (by registration date) in a period, summed per VAT rate: net, VAT and gross in the base currency and the number of documents, credit notes counting negative. The rows of `reports/vat-detail` grouped by rate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.vat_summary(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**side:** `typing.Optional[VatSummaryReportsRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">cash_flow</a>(...) -> CashFlowReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cash flow statement of a period from the posted transactions that touch a cash account: the inflow and outflow of every counterpart account, grouped into operating, investing and financing by the account prefixes of the company's chart template, with opening and closing cash and `balanced` telling whether opening cash plus the net change equals closing cash. Template account names follow the `Accept-Language` header.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.cash_flow(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">stock_aging</a>(...) -> StockAgingReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Age of the stock on hand at `asOf` per item and warehouse: the remaining quantity and value of each FIFO receipt layer, bucketed by days since the receipt (0 to 30, 31 to 60, 61 to 90, over 90), with totals; `warehouseId` limits the report to one warehouse. When movements after `asOf` exist, the layers are rebuilt by replaying the movements up to that date.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.stock_aging(
    as_of=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">stock_shortage</a>(...) -> StockShortageReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Items whose reserved quantity exceeds the quantity on hand, per warehouse: on hand, reserved and the shortage. Only items with a reservation are checked; `warehouseId` limits the report to one warehouse.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.stock_shortage()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">sie</a>(...) -> SieReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export the ledger of one financial year as an SIE file (the Swedish standard accounting interchange format, specification 4B). The file carries the chart of accounts, the opening and closing balance of every balance sheet account and the turnover of every result account for the year and the year before it, and, when asked for, every posted voucher of the year with its lines. Cost centres travel as dimension 1 and projects as dimension 6. Services that build a Swedish annual report read this file.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.sie(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**include_transactions:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">datev</a>(...) -> DatevReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export the posted ledger of a period as a DATEV Buchungsstapel file (DATEV format, category 21, version 700). Every transaction becomes one or more bookings of an amount between an account and a contra account; a transaction with more than two lines is split into pairs whose totals match it. The file is semicolon separated and written in the Windows-1252 character set DATEV expects.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.datev(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**consultant_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**client_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">fec</a>(...) -> FecReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export the posted ledger of a period as a French FEC file (fichier des écritures comptables, order of 29 July 2013). One line per journal entry line, with the eighteen fields the order names, in their order, after a header line. Tab separated, UTF-8, comma as the decimal separator.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.fec(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">eu_purchases</a>(...) -> EuPurchasesReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Registered purchase invoices of a period (by registration date) from partners in another EU country, summed per partner country and VAT rate: net and VAT in the base currency and the number of documents, credit notes counting negative. The partner's country is the country code of its address, else the first two characters of its VAT number.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.eu_purchases(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">vat_detail</a>(...) -> VatDetailReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

VAT of issued sale invoices (by issue date) or registered purchase invoices (by registration date) in a period, one row per document and VAT rate: net, VAT and gross in the base currency, with totals; credit notes count negative. `reports/vat-summary` groups these rows by rate.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.vat_detail(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**side:** `typing.Optional[VatDetailReportsRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">pos_sales</a>(...) -> PosSalesReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

POS reports of a period (by report date): per report the net, VAT, gross, cash and card amounts and the cost of goods sold, the net and VAT per VAT rate across the reports, and totals.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.pos_sales(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">online_sales</a>(...) -> OnlineSalesReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Sales orders created in a period, grouped by channel and currency: the number of orders, how many are fulfilled, cancelled or still open (new or reserved), and the net and gross of the orders that are not cancelled, computed from their lines.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.online_sales(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">oss</a>(...) -> OssReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Issued sale invoices and credit notes of a period (by issue date) to partners in another EU country, summed per partner country and VAT rate: net and VAT in the base currency and the number of documents. The partner's country is the country code of its address, else the first two characters of its VAT number.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.oss(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">advance_reconciliation</a>(...) -> AdvanceReconciliationReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Cash advances per employee for a period: the balance before `fromDate`, the advances paid out and returned through cash orders in the period, the amount settled by expense reports dated in the period, and the closing balance. A cash order counts as an advance when it names an employee and its counter account is the `cash.advances` posting rule.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.advance_reconciliation(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">write_off_acts</a>(...) -> WriteOffActsReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Stock issued by write-offs and stock takes in a period: one row per outgoing movement with item, warehouse, quantity, cost and notes, and the total cost; `warehouseId` limits the report to one warehouse.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.write_off_acts(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**warehouse_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">cost_centers</a>(...) -> CostCentersReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Income, expenses and result per cost centre for a period, from the posted journal lines assigned to a cost centre.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.cost_centers(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">cost_center_activity</a>(...) -> CostCenterActivityReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Posted journal lines of one cost centre for a period, summed per account: debit, credit and net. Template account names follow the `Accept-Language` header.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.cost_center_activity(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
    cost_center_id="costCenterId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**cost_center_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">cost_center_items</a>(...) -> CostCenterItemsReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Net purchases per cost centre and item for a period, from the lines of registered purchase invoices (by registration date) that carry a cost centre, credit notes counting negative; `costCenterId` limits the report to one cost centre. A line without an item is reported under its description.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.cost_center_items(
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**cost_center_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">jobs_create</a>(...) -> JobsCreateReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Queue a report to be built in the background in one or more formats (`json`, `xlsx`, `pdf`) and stored as files; the job is returned at once with status `queued`. `reportType` is one of trial-balance, partner-balances, debt-aging, stock-balance, vat-summary, vat-detail, eu-purchases, oss, pos-sales, online-sales, advance-reconciliation, write-off-acts, cost-centers, cost-center-activity, cost-center-items and cash-flow, and `params` is the body of that report route; an unknown type or invalid params are refused with 422. Follow the job with `reports/jobs/get`, download its outputs with `files/get`, and listen for `report.completed` or `report.failed`; a report that does not finish within ten minutes fails.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.jobs_create(
    report_type="reportType",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**report_type:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**params:** `typing.Optional[typing.Dict[str, typing.Any]]` 
    
</dd>
</dl>

<dl>
<dd>

**formats:** `typing.Optional[typing.List[JobsCreateReportsRequestFormatsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">jobs_get</a>(...) -> JobsGetReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one report job with its status (`queued`, `running`, `completed` or `failed`), the error of a failed job and the output files of a completed one.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.jobs_get(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">jobs_list</a>(...) -> JobsListReportsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the company's report jobs, newest first; filterable by `status` and `reportType`, sortable by `createdAt`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.jobs_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[typing.List[JobsListReportsRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[JobsListReportsRequestFilterItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**totals:** `typing.Optional[typing.List[str]]` — Numeric fields to sum over every row matching the filter (not only the current page)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## consolidation
<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">groups_create</a>(...) -> GroupsCreateConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a consolidation group owned by the calling company; `presentationCurrency` defaults to the company's base currency. Members are added with `consolidation/members/add`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.groups_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**presentation_currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">groups_list</a>() -> GroupsListConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the calling company's consolidation groups with their member counts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.groups_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">groups_get</a>(...) -> GroupsGetConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return one consolidation group with its members, each with its ownership percentage and consolidation method.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.groups_get(
    group_id="groupId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">groups_update</a>(...) -> GroupsUpdateConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Rename a consolidation group or change its presentation currency.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.groups_update(
    group_id="groupId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**presentation_currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">groups_delete</a>(...) -> GroupsDeleteConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a consolidation group.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.groups_delete(
    group_id="groupId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">members_add</a>(...) -> MembersAddConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Add a company to a consolidation group with its ownership percentage and method (`full`, `proportional` or `equity`), or change those of an existing member. Another company can be added only by a signed-in user who is owner, admin or accountant of it; an API key is refused with 403.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.members_add(
    group_id="groupId",
    member_company_id="memberCompanyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**member_company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**ownership_percent:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**method:** `typing.Optional[MembersAddConsolidationRequestMethod]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">members_remove</a>(...) -> MembersRemoveConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove a company from a consolidation group.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.members_remove(
    group_id="groupId",
    member_company_id="memberCompanyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**member_company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">intercompany_candidates</a>(...) -> IntercompanyCandidatesConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Partners in member companies that look like other members of the same group (matched on company code or VAT code), with any existing intercompany link. Confirming a candidate via intercompany/links/set enables invoice mirroring.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.intercompany_candidates(
    group_id="groupId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">intercompany_links_set</a>(...) -> IntercompanyLinksSetConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Confirm that a partner record in one member company represents another member company of the group. Once links exist in both directions, issuing an intercompany sale invoice automatically creates the matching draft purchase invoice in the counterparty.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.intercompany_links_set(
    group_id="groupId",
    partner_id="partnerId",
    counterparty_company_id="counterpartyCompanyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**counterparty_company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">intercompany_links_list</a>(...) -> IntercompanyLinksListConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the intercompany links of a group: which partner record of which member company stands for which other member company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.intercompany_links_list(
    group_id="groupId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">intercompany_links_remove</a>(...) -> IntercompanyLinksRemoveConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove an intercompany link from a group.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.intercompany_links_remove(
    group_id="groupId",
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">intercompany_report</a>(...) -> IntercompanyReportConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Intercompany reconciliation for a period: every issued intercompany sale invoice with its mirrored or manually recorded counterpart, unmatched documents on both sides, and per-currency totals with differences. Confirmed pairs are the basis for consolidation eliminations.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.intercompany_report(
    group_id="groupId",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">report</a>(...) -> ReportConsolidationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Consolidated financial statements of a group for a period in its presentation currency, with the consolidated trial balance and cash flow, each member's contribution and the intercompany candidates. Each member's balances are translated at the group owner's exchange rates of `toDate` and taken in full, in proportion to the ownership (`proportional`) or as an equity-method investment (`equity`); a fully consolidated member held below 100 % yields the non-controlling interest, and `eliminations` are amounts added to account codes before the statements are assembled (`balanced` tells whether they net to zero). Refused with 422 when the group has no members.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.report(
    group_id="groupId",
    from_date=datetime.date.fromisoformat("2026-07-01"),
    to_date=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**group_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[ReportConsolidationRequestCategory]` 
    
</dd>
</dl>

<dl>
<dd>

**eliminations:** `typing.Optional[typing.List[ReportConsolidationRequestEliminationsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## public
<details><summary><code>client.public.<a href="src/nordlet/public/client.py">integration_requests</a>(...) -> IntegrationRequestsPublicResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Store a request for an integration: the integration asked for and the sender's name, company, e-mail and details. When `website` is filled in, the call answers `received` without storing anything.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.public.integration_requests(
    integration="integration",
    name="name",
    email="email",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**integration:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**company:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**details:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**website:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.public.<a href="src/nordlet/public/client.py">pay</a>(...)</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Redirect (302) to the company's payment page for the issued invoice that carries this payment token, rendered from the template set with `sales/invoices/payment-settings/update` with the invoice number, the amount still unpaid, the currency, the token, the invoice id and the customer name (see `sales/invoices/payment-link`). Answers 404 when the token matches no issued invoice or the company has no template, and 409 when the invoice is already paid.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.public.pay(
    token="token",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**token:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## billing
<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">account_get</a>() -> AccountGetBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the signed-in user's billing account: plan, account type, status, balance, trial and payment state, the month-to-date usage of the companies the user pays for with an estimate of today's charge, the plan catalogue, and the top-up, automatic top-up and overdraft settings.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.account_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">account_set_plan</a>(...) -> AccountSetPlanBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the plan of the user's flat-rate billing account; answers 409 when the account type is not `flat_rate`. With a Stripe subscription and payments configured, the subscription is moved to the new plan.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.account_set_plan(
    plan="starter",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**plan:** `AccountSetPlanBillingRequestPlan` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">account_set_account_type</a>(...) -> AccountSetAccountTypeBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Switch the user's billing account between `flat_rate` and `per_request`. With a Stripe subscription and payments configured, the subscription is moved to the plan's price for `flat_rate`; for `per_request` the plan is taken off the subscription, and a subscription that carried only the plan is cancelled, leaving the account without one. When Stripe refuses the change, the previous account type is restored.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.account_set_account_type(
    account_type="flat_rate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**account_type:** `AccountSetAccountTypeBillingRequestAccountType` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">account_set_auto_top_up</a>(...) -> AccountSetAutoTopUpBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Switch automatic top-ups on or off and set their amount. Switching them on needs a Stripe customer, which the first card top-up creates (400 otherwise); when switched on, a top-up is charged at once if the balance is at or below zero, no payment has failed and no top-up was requested in the last 24 hours.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.account_set_auto_top_up(
    enabled=True,
    amount_cents=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**enabled:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**amount_cents:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">account_set_overdraft_cap</a>(...) -> AccountSetOverdraftCapBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the overdraft cap of the user's billing account: how far usage charges may take the balance below zero before the account is suspended. A suspended account whose balance is within the new cap is activated again.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.account_set_overdraft_cap(
    cap_cents=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cap_cents:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">topup_create</a>(...) -> TopupCreateBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Open a Stripe Checkout session for a one-time credit top-up of `amountCents` and return its URL; a Stripe customer is created for the user when there is none. `returnTo` chooses whether Checkout returns to the credits page or to the onboarding plan page, in `locale`. Answers 503 when online payments are not configured.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.topup_create(
    amount_cents=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**amount_cents:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[TopupCreateBillingRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**return_to:** `typing.Optional[TopupCreateBillingRequestReturnTo]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">topup_confirm</a>(...) -> TopupConfirmBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Confirm a paid top-up Checkout session by `sessionId` and credit the account at once instead of waiting for the Stripe webhook; a session is credited only once. Answers 404 when the session is not the user's own or is not paid.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.topup_confirm(
    session_id="sessionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**session_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">flat_rate_create</a>(...) -> FlatRateCreateBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Open a Stripe Checkout session for a flat-rate subscription on `plan`, with the trial period of `trialDays` days, and return its URL; a Stripe customer is created for the user when there is none. Answers 409 when a flat-rate subscription is already active and 503 when online payments are not configured or the plan has no price.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.flat_rate_create()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `typing.Optional[FlatRateCreateBillingRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**plan:** `typing.Optional[FlatRateCreateBillingRequestPlan]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">flat_rate_confirm</a>(...) -> FlatRateConfirmBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Confirm a completed flat-rate Checkout session by `sessionId`: the account becomes `flat_rate` on the session's plan with status `active` and the subscription attached, unless the Stripe webhook already did this. Answers 404 when the session is not the user's own or not completed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.flat_rate_confirm(
    session_id="sessionId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**session_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">portal_create</a>(...) -> PortalCreateBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Open a Stripe customer portal session that returns to the credits page in `locale`, and return its URL. Answers 503 when online payments are not configured and 400 when the user has no Stripe customer yet.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.portal_create()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `typing.Optional[PortalCreateBillingRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">transactions_list</a>(...) -> TransactionsListBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the newest credit transactions of the user's billing account, up to `limit`: trial grants, top-ups, usage charges, activations and adjustments, each with the balance after it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.transactions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">usage_list</a>(...) -> UsageListBillingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the daily usage records of the companies the user pays for, from `from` to `to`: one row per company, date and metric (API requests, OCR pages, file storage bytes, database bytes, sale invoices).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
import datetime

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.usage_list(
    from_=datetime.date.fromisoformat("2026-07-01"),
    to=datetime.date.fromisoformat("2026-07-01"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `datetime.date` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## account
<details><summary><code>client.account.<a href="src/nordlet/account/client.py">login_link_request</a>(...) -> LoginLinkRequestAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a sign-in link for the e-mail address and send it; the link is valid for 15 minutes and is consumed with `account/login-link/consume`. When an unused link was requested for the same address within the last minute, the call answers `sent` without sending another. `locale` sets the language of the e-mail and of the link; `app` set to `invoice` makes the link open the invoice app instead of the Nordlet app; `acceptTerms`, `acceptDpa` and `referralCode` are stored with the link and used when the address has no account yet.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.login_link_request(
    email="email",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[LoginLinkRequestAccountRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**accept_terms:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**accept_dpa:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**referral_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**app:** `typing.Optional[LoginLinkRequestAccountRequestApp]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">login_link_consume</a>(...) -> LoginLinkConsumeAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Exchange a sign-in link token for a session; an unknown, used or expired token is refused with 401. When no account has the address, one is created (`isNewUser`), which is refused with 422 unless the link was requested with `acceptTerms` and `acceptDpa`; a `referralCode` on the link records who referred the new user. A link from `account/email/change-request` changes the signed-in user's address instead, refused with 409 when another account has it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.login_link_consume(
    token="token",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**token:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">logout</a>() -> LogoutAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete the session the call was made with.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.logout()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">me</a>() -> MeAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the signed-in user, their active company and role in it, the companies they belong to and their consent state. `billing` is the billing account that pays for the active company (its payer, or the user when there is none or no company), with `isPayer` saying whether that is the user; `referralPoints` is the user's current points balance.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.me()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">members_list</a>() -> MembersListAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the members of the active company with their role.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.members_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">members_set_role</a>(...) -> MembersSetRoleAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the role of a member of the active company; owners and admins may call it. Refused with 422 for the caller's own role and with 403 for the owner's, which only `account/members/transfer-ownership` changes.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.members_set_role(
    user_id="userId",
    role="admin",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**user_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `MembersSetRoleAccountRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">members_transfer_ownership</a>(...) -> MembersTransferOwnershipAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Make another member the owner of the active company; the caller must be its owner and becomes an admin. Refused with 422 when `userId` is the caller. With `movePayer` the company's billing also moves to the new owner, which only the member currently paying for it may do (403).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.members_transfer_ownership(
    user_id="userId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**user_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**move_payer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">members_remove</a>(...) -> MembersRemoveAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Remove a member from the active company; owners and admins may call it. Their sessions lose this company as the active one and the API keys they created for it are revoked. Refused with 422 for the caller themself and with 403 for the owner.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.members_remove(
    user_id="userId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**user_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">invites_create</a>(...) -> InvitesCreateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an invitation to the active company for an e-mail address with the given role and send it by e-mail in `locale`; owners and admins may call it. The invitation is valid for 7 days and replaces an earlier pending one for the same address. Refused with 409 when the address already belongs to a member.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.invites_create(
    email="email",
    role="admin",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**role:** `InvitesCreateAccountRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvitesCreateAccountRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">invites_list</a>() -> InvitesListAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the pending invitations of the active company; `expired` marks those past their expiry.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.invites_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">invites_revoke</a>(...) -> InvitesRevokeAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a pending invitation of the active company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.invites_revoke(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">invites_get</a>(...) -> InvitesGetAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Read a pending invitation by its token: the invited address, role and company name, whether it has expired and whether an account with that address already exists (`userExists`), in which case `account/invites/accept` must be called signed in as that account.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.invites_get(
    token="token",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**token:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">invites_accept</a>(...) -> InvitesAcceptAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Accept an invitation and return a session with the invited company active. When the address has no account, one is created with `name` and `locale`, which is refused with 422 unless `acceptTerms` and `acceptDpa` are true; when it has one, the call must be made signed in as that account (401 otherwise). An expired invitation is refused with 422.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.invites_accept(
    token="token",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**token:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[InvitesAcceptAccountRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**accept_terms:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**accept_dpa:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">locale_set</a>(...) -> LocaleSetAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the user's language: with an active company it is stored on their membership of that company (`scope` = `membership`), otherwise on the user (`scope` = `user`).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.locale_set(
    locale="en",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `LocaleSetAccountRequestLocale` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_create</a>(...) -> CompaniesCreateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a company with the caller as its owner and payer, seed its chart of accounts from the template of `countryCode`, and make it the active company of the session. `timeZone` defaults to the country's, `isVatPayer` to true and `defaultInvoiceCurrency` to the base currency. Refused with 422 when `baseCurrency` is not a supported currency.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sme_exemption_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_vat_payer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_period:** `typing.Optional[CompaniesCreateAccountRequestVatPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**fiscal_year_end_month:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**time_zone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**filing_options:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[CompaniesCreateAccountRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**peppol_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sepa_creditor_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**default_invoice_currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**legal_form:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**registry_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**incorporated_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**share_capital:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts_kept_by:** `typing.Optional[CompaniesCreateAccountRequestAccountsKeptBy]` 
    
</dd>
</dl>

<dl>
<dd>

**bookkeeper_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**audit_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**country_code:** `typing.Optional[CompaniesCreateAccountRequestCountryCode]` — Jurisdiction the company is registered in (immutable after creation)
    
</dd>
</dl>

<dl>
<dd>

**base_currency:** `typing.Optional[str]` — Currency the ledger is kept in; defaults to the national currency of countryCode (immutable after creation)
    
</dd>
</dl>

<dl>
<dd>

**is_sandbox:** `typing.Optional[bool]` — Sandbox companies hold test data and are purged immediately on delete (immutable after creation)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_select</a>(...) -> CompaniesSelectAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Make one of the caller's companies the active company of the session. Refused with 403 when the caller is not a member and with 422 when the company is archived or deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_select(
    company_id="companyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_profile</a>() -> CompaniesProfileAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the profile of the active company.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_profile()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_update</a>(...) -> CompaniesUpdateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Change the profile of the active company; owners and admins may call it. Only the fields sent are changed, and the nullable ones can be sent as null to clear them. `logo` stores a base64-encoded image as a file of the company and sets `logoFileId`. The country, base currency and sandbox flag are fixed at creation.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_update()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sme_exemption_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**is_vat_payer:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_period:** `typing.Optional[CompaniesUpdateAccountRequestVatPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**fiscal_year_end_month:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**time_zone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**filing_options:** `typing.Optional[typing.Dict[str, typing.Optional[str]]]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[CompaniesUpdateAccountRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**email:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**iban:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**bank_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**peppol_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**sepa_creditor_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**default_invoice_currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**legal_form:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**registry_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**incorporated_on:** `typing.Optional[datetime.date]` 
    
</dd>
</dl>

<dl>
<dd>

**share_capital:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts_kept_by:** `typing.Optional[CompaniesUpdateAccountRequestAccountsKeptBy]` 
    
</dd>
</dl>

<dl>
<dd>

**bookkeeper_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**auditor_registration_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**audit_required:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**logo:** `typing.Optional[CompaniesUpdateAccountRequestLogo]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_archive</a>(...) -> CompaniesArchiveAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the company named by `companyId` to `archived`; the caller must be its owner. Every session that had it active loses it. Refused with 409 unless the company is active; `account/companies/activate` reverses it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_archive(
    company_id="companyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_delete</a>(...) -> CompaniesDeleteAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the company named by `companyId` to `deleted`; the caller must be its owner, and every session that had it active loses it. A sandbox company is purged at once; any other is purged by the scheduled purge after `purgeAfter` (10 days) and can be restored until then with `account/companies/activate`. Refused with 409 when it is already deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_delete(
    company_id="companyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">companies_activate</a>(...) -> CompaniesActivateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set an archived or deleted company named by `companyId` back to `active`; the caller must be its owner. Refused with 409 when it is already active.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.companies_activate(
    company_id="companyId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**company_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">api_keys_create</a>(...) -> ApiKeysCreateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create an API key for the active company and return the key itself once; owners, admins and developers may call it. `scopes` defaults to the caller's own scopes and may not exceed them (403); without `expiresInDays` the key does not expire.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.api_keys_create(
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**scopes:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**expires_in_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">api_keys_list</a>() -> ApiKeysListAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the API keys of the active company, including expired and revoked ones.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.api_keys_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">api_keys_rotate</a>(...) -> ApiKeysRotateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a new key with the name and scopes of the key `id` and return it once; the old key keeps working for `overlapHours` and then expires, and its `replacedByKeyId` points to the new one. `expiresInDays` applies to the new key. Refused with 409 when the old key is revoked.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.api_keys_rotate(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**overlap_hours:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**expires_in_days:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">api_keys_revoke</a>(...) -> ApiKeysRevokeAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Revoke an API key of the active company at once.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.api_keys_revoke(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">consent_accept</a>(...) -> ConsentAcceptAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Record the signed-in user's acceptance of the current Terms of Service and Data Processing Agreement versions and return the consent state.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.consent_accept(
    accept_terms=True,
    accept_dpa=True,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**accept_terms:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**accept_dpa:** `bool` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">profile_update</a>(...) -> ProfileUpdateAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Set the signed-in user's name; null or a blank string clears it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.profile_update()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">email_change_request</a>(...) -> EmailChangeRequestAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Send a confirmation link to `newEmail`; the address changes when that link is consumed with `account/login-link/consume`. When an unused link was sent to the address within the last minute, the call answers `sent` without sending another. Refused with 422 when it is already the user's address and with 409 when another account has it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.email_change_request(
    new_email="newEmail",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**new_email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[EmailChangeRequestAccountRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">sessions_list</a>() -> SessionsListAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the signed-in user's sessions that have not expired; `current` marks the one the call was made with.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.sessions_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">sessions_revoke</a>(...) -> SessionsRevokeAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete one of the signed-in user's sessions.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.sessions_revoke(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">sessions_revoke_others</a>() -> SessionsRevokeOthersAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete every session of the signed-in user except the one the call was made with, and return how many were deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.sessions_revoke_others()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">export</a>() -> ExportAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the user's profile, consent state, memberships, unexpired sessions, billing account, credit transactions and the audit entries they made in their companies (the most recent 5000 of each of the last two).
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.export()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">delete</a>(...) -> DeleteAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the user: sessions, sign-in links, memberships and pending invitations are deleted at once; the email and name are replaced by an anonymous placeholder immediately and the remaining row is removed after 30 days. Refused while the user still owns or pays for a company that is not deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.delete(
    confirm_email="confirmEmail",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**confirm_email:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">referral_get</a>() -> ReferralGetAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the user's referral code (allocated on first call) and sign-up link, their points balance, the number of accounts they referred and the last 50 points entries. `rates.perEur` is the points the referrer earns per euro a referred user tops up, `rates.pointCents` the credit one point converts to with `account/referral/convert`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.referral_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">referral_convert</a>(...) -> ReferralConvertAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Convert `points` of the user's referral points into credit on their billing account at `rates.pointCents` per point, booked as an `adjustment` credit transaction; a billing account past its trial is set to active when the new balance allows. Refused with 422 when the user has fewer points than requested.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.referral_convert(
    points=1000000,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**points:** `int` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">table_settings_get</a>(...) -> TableSettingsGetAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Return the signed-in user's saved column list and page size for the table `tableKey`; both are null when nothing is saved.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.table_settings_get(
    table_key="tableKey",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**table_key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">table_settings_set</a>(...) -> TableSettingsSetAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Save the signed-in user's column list and page size for the table `tableKey`; only the fields sent are changed, and null clears one.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.table_settings_set(
    table_key="tableKey",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**table_key:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**columns:** `typing.Optional[typing.List[str]]` 
    
</dd>
</dl>

<dl>
<dd>

**page_size:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">table_settings_list</a>() -> TableSettingsListAccountResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List the signed-in user's saved table settings.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.table_settings_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

