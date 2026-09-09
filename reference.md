# Reference
## Reference
<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_exchange_rates_sync</a>(...) -> PostV1ReferenceExchangeRatesSyncResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_exchange_rates_sync()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_exchange_rates_list</a>(...) -> PostV1ReferenceExchangeRatesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_exchange_rates_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceExchangeRatesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceExchangeRatesListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_exchange_rates_set</a>(...) -> PostV1ReferenceExchangeRatesSetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_exchange_rates_set(
    currency="currency",
    date="date",
    rate="rate",
)

```
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

**date:** `str` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_exchange_rates_overrides_list</a>(...) -> PostV1ReferenceExchangeRatesOverridesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_exchange_rates_overrides_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceExchangeRatesOverridesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceExchangeRatesOverridesListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_exchange_rates_overrides_delete</a>(...) -> PostV1ReferenceExchangeRatesOverridesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_exchange_rates_overrides_delete(
    currency="currency",
    date="date",
)

```
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_countries_list</a>() -> PostV1ReferenceCountriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_countries_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_lt_counties_list</a>() -> PostV1ReferenceLtCountiesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_lt_counties_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_lt_municipalities_list</a>(...) -> PostV1ReferenceLtMunicipalitiesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_lt_municipalities_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_lt_cities_list</a>(...) -> PostV1ReferenceLtCitiesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_lt_cities_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_banks_list</a>(...) -> PostV1ReferenceBanksListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_banks_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceBanksListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceBanksListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_banks_upsert</a>(...) -> PostV1ReferenceBanksUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_banks_upsert(
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_lt_regions_list</a>() -> PostV1ReferenceLtRegionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_lt_regions_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_currencies_list</a>(...) -> PostV1ReferenceCurrenciesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_currencies_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceCurrenciesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceCurrenciesListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_vat_classifiers_list</a>(...) -> PostV1ReferenceVatClassifiersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_vat_classifiers_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceVatClassifiersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceVatClassifiersListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_vat_classifiers_upsert</a>(...) -> PostV1ReferenceVatClassifiersUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.reference import PostV1ReferenceVatClassifiersUpsertRequestRowsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_vat_classifiers_upsert(
    rows=[
        PostV1ReferenceVatClassifiersUpsertRequestRowsItem(
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

**rows:** `typing.List[PostV1ReferenceVatClassifiersUpsertRequestRowsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_eu_vat_rates_list</a>(...) -> PostV1ReferenceEuVatRatesListResponse</code></summary>
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

client.reference.post_v1reference_eu_vat_rates_list()

```
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

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_eu_vat_rates_set_overrides</a>(...) -> PostV1ReferenceEuVatRatesSetOverridesResponse</code></summary>
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
from nordlet.reference import PostV1ReferenceEuVatRatesSetOverridesRequestRatesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_eu_vat_rates_set_overrides(
    country_code="countryCode",
    rates=[
        PostV1ReferenceEuVatRatesSetOverridesRequestRatesItem(
            category="standard",
            rate_percent="ratePercent",
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

**rates:** `typing.List[PostV1ReferenceEuVatRatesSetOverridesRequestRatesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_vat_resolve</a>(...) -> PostV1ReferenceVatResolveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_vat_resolve()

```
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

**supply_type:** `typing.Optional[PostV1ReferenceVatResolveRequestSupplyType]` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_cn_codes_list</a>(...) -> PostV1ReferenceCnCodesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_cn_codes_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceCnCodesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceCnCodesListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_cn_codes_upsert</a>(...) -> PostV1ReferenceCnCodesUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.reference import PostV1ReferenceCnCodesUpsertRequestRowsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_cn_codes_upsert(
    rows=[
        PostV1ReferenceCnCodesUpsertRequestRowsItem(
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

**rows:** `typing.List[PostV1ReferenceCnCodesUpsertRequestRowsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_compliance_versions_list</a>(...) -> PostV1ReferenceComplianceVersionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_compliance_versions_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_intrastat_thresholds_list</a>() -> PostV1ReferenceIntrastatThresholdsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_intrastat_thresholds_list()

```
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_units_list</a>(...) -> PostV1ReferenceUnitsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_units_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceUnitsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceUnitsListRequestFilterItem]]` 
    
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_series_create</a>(...) -> PostV1ReferenceSeriesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_series_create(
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

<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">post_v1reference_series_list</a>(...) -> PostV1ReferenceSeriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reference.post_v1reference_series_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReferenceSeriesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReferenceSeriesListRequestFilterItem]]` 
    
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

## Partners
<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_addresses_create</a>(...) -> PostV1PartnersAddressesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_addresses_create(
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

**type:** `typing.Optional[PostV1PartnersAddressesCreateRequestType]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_addresses_update</a>(...) -> PostV1PartnersAddressesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_addresses_update(
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

**type:** `typing.Optional[PostV1PartnersAddressesUpdateRequestType]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_addresses_delete</a>(...) -> PostV1PartnersAddressesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_addresses_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_addresses_list</a>(...) -> PostV1PartnersAddressesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_addresses_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersAddressesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersAddressesListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_contacts_create</a>(...) -> PostV1PartnersContactsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_contacts_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_contacts_update</a>(...) -> PostV1PartnersContactsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_contacts_update(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_contacts_delete</a>(...) -> PostV1PartnersContactsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_contacts_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_contacts_list</a>(...) -> PostV1PartnersContactsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_contacts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersContactsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersContactsListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_bank_accounts_create</a>(...) -> PostV1PartnersBankAccountsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_bank_accounts_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_bank_accounts_update</a>(...) -> PostV1PartnersBankAccountsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_bank_accounts_update(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_bank_accounts_delete</a>(...) -> PostV1PartnersBankAccountsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_bank_accounts_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_bank_accounts_list</a>(...) -> PostV1PartnersBankAccountsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_bank_accounts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersBankAccountsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersBankAccountsListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_files_list</a>(...) -> PostV1PartnersFilesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_files_list(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">reminders_the_overnight_debt_reminder_job_would_send_today_for_this_company</a>() -> PostV1PartnersDebtRemindersPreviewResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.reminders_the_overnight_debt_reminder_job_would_send_today_for_this_company()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_debt_reminders_list</a>(...) -> PostV1PartnersDebtRemindersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_debt_reminders_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersDebtRemindersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersDebtRemindersListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_validate_vat</a>(...) -> PostV1PartnersValidateVatResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_validate_vat()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_vat_reviews_list</a>(...) -> PostV1PartnersVatReviewsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_vat_reviews_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersVatReviewsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersVatReviewsListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_vat_reviews_resolve</a>(...) -> PostV1PartnersVatReviewsResolveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_vat_reviews_resolve(
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

**resolution:** `PostV1PartnersVatReviewsResolveRequestResolution` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_create</a>(...) -> PostV1PartnersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_create(
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

**type:** `typing.Optional[PostV1PartnersCreateRequestType]` 
    
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

**birth_date:** `typing.Optional[str]` 
    
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

**address:** `typing.Optional[PostV1PartnersCreateRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[PostV1PartnersCreateRequestCorrespondenceAddress]` 
    
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

**other_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**foreign_tax_number:** `typing.Optional[str]` 
    
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

**first_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[str]` 
    
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

**legal_country_class:** `typing.Optional[PostV1PartnersCreateRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_find_or_create</a>(...) -> PostV1PartnersFindOrCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_find_or_create(
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

**type:** `typing.Optional[PostV1PartnersFindOrCreateRequestType]` 
    
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

**birth_date:** `typing.Optional[str]` 
    
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

**address:** `typing.Optional[PostV1PartnersFindOrCreateRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[PostV1PartnersFindOrCreateRequestCorrespondenceAddress]` 
    
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

**other_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**foreign_tax_number:** `typing.Optional[str]` 
    
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

**first_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[str]` 
    
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

**legal_country_class:** `typing.Optional[PostV1PartnersFindOrCreateRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_get</a>(...) -> PostV1PartnersGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_get(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_update</a>(...) -> PostV1PartnersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_update(
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

**type:** `typing.Optional[PostV1PartnersUpdateRequestType]` 
    
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

**birth_date:** `typing.Optional[str]` 
    
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

**address:** `typing.Optional[PostV1PartnersUpdateRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**correspondence_address:** `typing.Optional[PostV1PartnersUpdateRequestCorrespondenceAddress]` 
    
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

**other_code:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**foreign_tax_number:** `typing.Optional[str]` 
    
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

**first_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**last_call_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**next_call_date:** `typing.Optional[str]` 
    
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

**legal_country_class:** `typing.Optional[PostV1PartnersUpdateRequestLegalCountryClass]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_delete</a>(...) -> PostV1PartnersDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">blank_a_partners_personal_data_and_hide_the_record</a>(...) -> PostV1PartnersAnonymizeResponse</code></summary>
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

client.partners.blank_a_partners_personal_data_and_hide_the_record(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_list</a>(...) -> PostV1PartnersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_groups_create</a>(...) -> PostV1PartnersGroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_groups_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_groups_update</a>(...) -> PostV1PartnersGroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_groups_update(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_groups_delete</a>(...) -> PostV1PartnersGroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_groups_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_groups_list</a>() -> PostV1PartnersGroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_groups_list()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_statuses_create</a>(...) -> PostV1PartnersStatusesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_statuses_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_statuses_update</a>(...) -> PostV1PartnersStatusesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_statuses_update(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_statuses_delete</a>(...) -> PostV1PartnersStatusesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_statuses_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_statuses_list</a>() -> PostV1PartnersStatusesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_statuses_list()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_inquiries_create</a>(...) -> PostV1PartnersInquiriesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_inquiries_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_inquiries_update</a>(...) -> PostV1PartnersInquiriesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_inquiries_update(
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

**status:** `typing.Optional[PostV1PartnersInquiriesUpdateRequestStatus]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_inquiries_get</a>(...) -> PostV1PartnersInquiriesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_inquiries_get(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_inquiries_list</a>(...) -> PostV1PartnersInquiriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_inquiries_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PartnersInquiriesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PartnersInquiriesListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1partners_credit_check</a>(...) -> PostV1PartnersCreditCheckResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1partners_credit_check(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_create</a>(...) -> PostV1LeadsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_create(
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

**status:** `typing.Optional[PostV1LeadsCreateRequestStatus]` 
    
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

**documents:** `typing.Optional[typing.List[PostV1LeadsCreateRequestDocumentsItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_get</a>(...) -> PostV1LeadsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_get(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_update</a>(...) -> PostV1LeadsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_update(
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

**status:** `typing.Optional[PostV1LeadsUpdateRequestStatus]` 
    
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

**documents:** `typing.Optional[typing.List[PostV1LeadsUpdateRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_delete</a>(...) -> PostV1LeadsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_list</a>(...) -> PostV1LeadsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LeadsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LeadsListRequestFilterItem]]` 
    
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_notes_create</a>(...) -> PostV1LeadsNotesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_notes_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_notes_delete</a>(...) -> PostV1LeadsNotesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_notes_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_notes_list</a>(...) -> PostV1LeadsNotesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_notes_list(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_files_list</a>(...) -> PostV1LeadsFilesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_files_list(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_sources_create</a>(...) -> PostV1LeadsSourcesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_sources_create(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_sources_update</a>(...) -> PostV1LeadsSourcesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_sources_update(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_sources_delete</a>(...) -> PostV1LeadsSourcesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_sources_delete(
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_sources_list</a>() -> PostV1LeadsSourcesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_sources_list()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_sources_options</a>() -> PostV1LeadsSourcesOptionsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.partners.post_v1leads_sources_options()

```
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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">post_v1leads_convert</a>(...) -> PostV1LeadsConvertResponse</code></summary>
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

client.partners.post_v1leads_convert(
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

**partner_type:** `typing.Optional[PostV1LeadsConvertRequestPartnerType]` 
    
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

## Catalog
<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_create</a>(...) -> PostV1CatalogItemsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_create(
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

**type:** `typing.Optional[PostV1CatalogItemsCreateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**tracking:** `typing.Optional[PostV1CatalogItemsCreateRequestTracking]` 
    
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

**translations:** `typing.Optional[typing.Dict[str, PostV1CatalogItemsCreateRequestTranslationsValue]]` 
    
</dd>
</dl>

<dl>
<dd>

**components:** `typing.Optional[typing.List[PostV1CatalogItemsCreateRequestComponentsItem]]` 
    
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

**price_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_to:** `typing.Optional[str]` 
    
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

**certificate_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_to:** `typing.Optional[str]` 
    
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_get</a>(...) -> PostV1CatalogItemsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_get(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_update</a>(...) -> PostV1CatalogItemsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_update(
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

**type:** `typing.Optional[PostV1CatalogItemsUpdateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**tracking:** `typing.Optional[PostV1CatalogItemsUpdateRequestTracking]` 
    
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

**translations:** `typing.Optional[typing.Dict[str, typing.Optional[PostV1CatalogItemsUpdateRequestTranslationsValue]]]` 
    
</dd>
</dl>

<dl>
<dd>

**components:** `typing.Optional[typing.List[PostV1CatalogItemsUpdateRequestComponentsItem]]` 
    
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

**price_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price_to:** `typing.Optional[str]` 
    
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

**certificate_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_to:** `typing.Optional[str]` 
    
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_delete</a>(...) -> PostV1CatalogItemsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_delete(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_list</a>(...) -> PostV1CatalogItemsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1CatalogItemsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1CatalogItemsListRequestFilterItem]]` 
    
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_files_list</a>(...) -> PostV1CatalogItemsFilesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_files_list(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_kinds_create</a>(...) -> PostV1CatalogItemsKindsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_kinds_create(
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

**saft_type:** `typing.Optional[PostV1CatalogItemsKindsCreateRequestSaftType]` 
    
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_kinds_update</a>(...) -> PostV1CatalogItemsKindsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_kinds_update(
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

**saft_type:** `typing.Optional[PostV1CatalogItemsKindsUpdateRequestSaftType]` 
    
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_kinds_delete</a>(...) -> PostV1CatalogItemsKindsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_kinds_delete(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_kinds_list</a>() -> PostV1CatalogItemsKindsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_kinds_list()

```
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_units_create</a>(...) -> PostV1CatalogUnitsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_units_create(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_units_update</a>(...) -> PostV1CatalogUnitsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_units_update(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_units_delete</a>(...) -> PostV1CatalogUnitsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_units_delete(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_units_list</a>() -> PostV1CatalogUnitsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_units_list()

```
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_units_options</a>(...) -> PostV1CatalogUnitsOptionsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_units_options()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `typing.Optional[PostV1CatalogUnitsOptionsRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_item_groups_create</a>(...) -> PostV1CatalogItemGroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_item_groups_create(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_item_groups_update</a>(...) -> PostV1CatalogItemGroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_item_groups_update(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_item_groups_delete</a>(...) -> PostV1CatalogItemGroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_item_groups_delete(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_item_groups_list</a>() -> PostV1CatalogItemGroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_item_groups_list()

```
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_suppliers_upsert</a>(...) -> PostV1CatalogItemsSuppliersUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_suppliers_upsert(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_suppliers_list</a>(...) -> PostV1CatalogItemsSuppliersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_suppliers_list()

```
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_items_suppliers_delete</a>(...) -> PostV1CatalogItemsSuppliersDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_items_suppliers_delete(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_create</a>(...) -> PostV1CatalogPriceListsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_create(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_update</a>(...) -> PostV1CatalogPriceListsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_update(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_list</a>() -> PostV1CatalogPriceListsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_list()

```
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_items_set</a>(...) -> PostV1CatalogPriceListsItemsSetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.catalog import PostV1CatalogPriceListsItemsSetRequestItemsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_items_set(
    price_list_id="priceListId",
    items=[
        PostV1CatalogPriceListsItemsSetRequestItemsItem(
            item_id="itemId",
            unit_price_excl_vat="unitPriceExclVat",
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

**items:** `typing.List[PostV1CatalogPriceListsItemsSetRequestItemsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_items_list</a>(...) -> PostV1CatalogPriceListsItemsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_items_list(
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

<details><summary><code>client.catalog.<a href="src/nordlet/catalog/client.py">post_v1catalog_price_lists_items_delete</a>(...) -> PostV1CatalogPriceListsItemsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.catalog.post_v1catalog_price_lists_items_delete(
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

## Sales
<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_create</a>(...) -> PostV1SalesInvoicesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.sales import PostV1SalesInvoicesCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_create(
    partner_id="partnerId",
    lines=[
        PostV1SalesInvoicesCreateRequestLinesItem()
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

**lines:** `typing.List[PostV1SalesInvoicesCreateRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[PostV1SalesInvoicesCreateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**credited_invoice_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[PostV1SalesInvoicesCreateRequestVatScheme]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_get</a>(...) -> PostV1SalesInvoicesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_get(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_pdf</a>(...) -> PostV1SalesInvoicesPdfResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_pdf(
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

**locale:** `typing.Optional[PostV1SalesInvoicesPdfRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_send</a>(...) -> PostV1SalesInvoicesSendResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_send(
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

**locale:** `typing.Optional[PostV1SalesInvoicesSendRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_peppol_xml</a>(...) -> PostV1SalesInvoicesPeppolXmlResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_peppol_xml(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_peppol_send</a>(...) -> PostV1SalesInvoicesPeppolSendResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_peppol_send(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_einvoice_xml</a>(...) -> PostV1SalesInvoicesEinvoiceXmlResponse</code></summary>
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

client.sales.post_v1sales_invoices_einvoice_xml(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_einvoice_send</a>(...) -> PostV1SalesInvoicesEinvoiceSendResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Build the national e-invoicing payload and deliver it to the bridge endpoint configured for the country gateway in compliance settings. The bridge (an accredited intermediary or connector) handles the certified national channel - SdI accreditation, KSeF sessions or ANAF SPV OAuth.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_einvoice_send(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_update</a>(...) -> PostV1SalesInvoicesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_update(
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

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**issue_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**vat_scheme:** `typing.Optional[PostV1SalesInvoicesUpdateRequestVatScheme]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1SalesInvoicesUpdateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_delete</a>(...) -> PostV1SalesInvoicesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_delete(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_issue</a>(...) -> PostV1SalesInvoicesIssueResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_issue(
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

**issue_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_lock</a>(...) -> PostV1SalesInvoicesLockResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_lock(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_unlock</a>(...) -> PostV1SalesInvoicesUnlockResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_unlock(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_payment_link</a>(...) -> PostV1SalesInvoicesPaymentLinkResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_payment_link(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_payment_settings_get</a>() -> PostV1SalesInvoicesPaymentSettingsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_payment_settings_get()

```
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_payment_settings_update</a>(...) -> PostV1SalesInvoicesPaymentSettingsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_payment_settings_update()

```
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_schedules_list</a>(...) -> PostV1SalesRecognitionSchedulesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_schedules_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1SalesRecognitionSchedulesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1SalesRecognitionSchedulesListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_apply_advance</a>(...) -> PostV1SalesInvoicesApplyAdvanceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_apply_advance(
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

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_invoices_list</a>(...) -> PostV1SalesInvoicesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_invoices_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1SalesInvoicesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1SalesInvoicesListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_create</a>(...) -> PostV1SalesActsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_create(
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

**type:** `typing.Optional[PostV1SalesActsCreateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1SalesActsCreateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_update</a>(...) -> PostV1SalesActsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_update(
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

**type:** `typing.Optional[PostV1SalesActsUpdateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**document_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1SalesActsUpdateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_issue</a>(...) -> PostV1SalesActsIssueResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_issue(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_cancel</a>(...) -> PostV1SalesActsCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_cancel(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_get</a>(...) -> PostV1SalesActsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_get(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_list</a>(...) -> PostV1SalesActsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1SalesActsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1SalesActsListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_acts_pdf</a>(...) -> PostV1SalesActsPdfResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_acts_pdf(
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

**locale:** `typing.Optional[PostV1SalesActsPdfRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1operation_types_create</a>(...) -> PostV1OperationTypesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1operation_types_create(
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

**invoice_type:** `typing.Optional[PostV1OperationTypesCreateRequestInvoiceType]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1operation_types_update</a>(...) -> PostV1OperationTypesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1operation_types_update(
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

**invoice_type:** `typing.Optional[PostV1OperationTypesUpdateRequestInvoiceType]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1operation_types_get</a>(...) -> PostV1OperationTypesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1operation_types_get(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1operation_types_delete</a>(...) -> PostV1OperationTypesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1operation_types_delete(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1operation_types_list</a>(...) -> PostV1OperationTypesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1operation_types_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1OperationTypesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1OperationTypesListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1document_series_create</a>(...) -> PostV1DocumentSeriesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1document_series_create(
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

**document_type:** `typing.Optional[PostV1DocumentSeriesCreateRequestDocumentType]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1document_series_update</a>(...) -> PostV1DocumentSeriesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1document_series_update(
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

**document_type:** `typing.Optional[PostV1DocumentSeriesUpdateRequestDocumentType]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1document_series_get</a>(...) -> PostV1DocumentSeriesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1document_series_get(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1document_series_delete</a>(...) -> PostV1DocumentSeriesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1document_series_delete(
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1document_series_list</a>(...) -> PostV1DocumentSeriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1document_series_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1DocumentSeriesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1DocumentSeriesListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_compute</a>(...) -> PostV1SalesRecognitionComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_compute()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_run</a>(...) -> PostV1SalesRecognitionRunResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_run()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**posting_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_progress</a>(...) -> PostV1SalesRecognitionProgressResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_progress(
    invoice_line_id="invoiceLineId",
    percent_complete="percentComplete",
)

```
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

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_modify</a>(...) -> PostV1SalesRecognitionModifyResponse</code></summary>
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

client.sales.post_v1sales_recognition_modify(
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

**approach:** `PostV1SalesRecognitionModifyRequestApproach` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**new_end_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**new_milestones:** `typing.Optional[typing.List[PostV1SalesRecognitionModifyRequestNewMilestonesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_runs_list</a>(...) -> PostV1SalesRecognitionRunsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_runs_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1SalesRecognitionRunsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1SalesRecognitionRunsListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_recognition_summary</a>(...) -> PostV1SalesRecognitionSummaryResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_recognition_summary()

```
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_refund_liability_list</a>(...) -> PostV1SalesRefundLiabilityListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_refund_liability_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1SalesRefundLiabilityListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1SalesRefundLiabilityListRequestFilterItem]]` 
    
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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">post_v1sales_refund_liability_true_up</a>(...) -> PostV1SalesRefundLiabilityTrueUpResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.sales.post_v1sales_refund_liability_true_up(
    invoice_id="invoiceId",
    estimated_total="estimatedTotal",
)

```
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

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Purchases
<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_create</a>(...) -> PostV1PurchasesInvoicesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.purchases import PostV1PurchasesInvoicesCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_create(
    partner_id="partnerId",
    document_number="documentNumber",
    document_date="documentDate",
    lines=[
        PostV1PurchasesInvoicesCreateRequestLinesItem()
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

**document_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[PostV1PurchasesInvoicesCreateRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[PostV1PurchasesInvoicesCreateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_get</a>(...) -> PostV1PurchasesInvoicesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_get(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_update</a>(...) -> PostV1PurchasesInvoicesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_update(
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

**document_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1PurchasesInvoicesUpdateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_delete</a>(...) -> PostV1PurchasesInvoicesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_delete(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_register</a>(...) -> PostV1PurchasesInvoicesRegisterResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_register(
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

**registration_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_list</a>(...) -> PostV1PurchasesInvoicesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PurchasesInvoicesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PurchasesInvoicesListRequestFilterItem]]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_create</a>(...) -> PostV1PurchasesOrdersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.purchases import PostV1PurchasesOrdersCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_create(
    partner_id="partnerId",
    order_date="orderDate",
    lines=[
        PostV1PurchasesOrdersCreateRequestLinesItem()
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

**order_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[PostV1PurchasesOrdersCreateRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**order_number:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expected_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_update</a>(...) -> PostV1PurchasesOrdersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_update(
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

**order_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**expected_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1PurchasesOrdersUpdateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_get</a>(...) -> PostV1PurchasesOrdersGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_get(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_list</a>(...) -> PostV1PurchasesOrdersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PurchasesOrdersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PurchasesOrdersListRequestFilterItem]]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_submit</a>(...) -> PostV1PurchasesOrdersSubmitResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_submit(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_approve</a>(...) -> PostV1PurchasesOrdersApproveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_approve(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_reject</a>(...) -> PostV1PurchasesOrdersRejectResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_reject(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_cancel</a>(...) -> PostV1PurchasesOrdersCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_cancel(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_close</a>(...) -> PostV1PurchasesOrdersCloseResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_close(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_orders_delete</a>(...) -> PostV1PurchasesOrdersDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_orders_delete(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_receipts_create</a>(...) -> PostV1PurchasesReceiptsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.purchases import PostV1PurchasesReceiptsCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_receipts_create(
    order_id="orderId",
    receipt_date="receiptDate",
    lines=[
        PostV1PurchasesReceiptsCreateRequestLinesItem(
            order_line_id="orderLineId",
            quantity="quantity",
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

**receipt_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[PostV1PurchasesReceiptsCreateRequestLinesItem]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_receipts_get</a>(...) -> PostV1PurchasesReceiptsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_receipts_get(
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_receipts_list</a>(...) -> PostV1PurchasesReceiptsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_receipts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PurchasesReceiptsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PurchasesReceiptsListRequestFilterItem]]` 
    
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

<details><summary><code>client.purchases.<a href="src/nordlet/purchases/client.py">post_v1purchases_invoices_match</a>(...) -> PostV1PurchasesInvoicesMatchResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.purchases.post_v1purchases_invoices_match(
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

## Capture
<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_settings_get</a>() -> PostV1CaptureSettingsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_settings_get()

```
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_settings_update</a>(...) -> PostV1CaptureSettingsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_settings_update()

```
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_settings_regenerate_intake</a>() -> PostV1CaptureSettingsRegenerateIntakeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_settings_regenerate_intake()

```
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">receive_an_inbound_email_with_supplier_documents_attached_postmark_style_or_generic_json</a>(...) -> PostV1CaptureInboundEmailResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.receive_an_inbound_email_with_supplier_documents_attached_postmark_style_or_generic_json()

```
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

**to_full:** `typing.Optional[typing.List[PostV1CaptureInboundEmailRequestToFullItem]]` 
    
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

**postmark_attachments:** `typing.Optional[typing.List[PostV1CaptureInboundEmailRequestAttachmentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `typing.Optional[PostV1CaptureInboundEmailRequestTo]` 
    
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

**attachments:** `typing.Optional[typing.List[PostV1CaptureInboundEmailRequestAttachmentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">read_a_vendor_bill_or_receipt_and_return_an_editable_purchase_invoice_draft</a>(...) -> PostV1CaptureDocumentsUploadResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.read_a_vendor_bill_or_receipt_and_return_an_editable_purchase_invoice_draft(
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">re_read_a_stored_capture_replacing_the_previous_draft</a>(...) -> PostV1CaptureDocumentsExtractResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.re_read_a_stored_capture_replacing_the_previous_draft(
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_documents_get</a>(...) -> PostV1CaptureDocumentsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_documents_get(
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_documents_list</a>(...) -> PostV1CaptureDocumentsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_documents_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1CaptureDocumentsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1CaptureDocumentsListRequestFilterItem]]` 
    
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">post_v1capture_documents_delete</a>(...) -> PostV1CaptureDocumentsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.post_v1capture_documents_delete(
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

<details><summary><code>client.capture.<a href="src/nordlet/capture/client.py">save_the_reviewed_draft_as_a_purchase_invoice_and_attach_the_original_document</a>(...) -> PostV1CaptureDocumentsConfirmResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.capture import PostV1CaptureDocumentsConfirmRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.capture.save_the_reviewed_draft_as_a_purchase_invoice_and_attach_the_original_document(
    id="id",
    document_number="documentNumber",
    document_date="documentDate",
    lines=[
        PostV1CaptureDocumentsConfirmRequestLinesItem()
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

**document_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[PostV1CaptureDocumentsConfirmRequestLinesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**partner_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**new_supplier:** `typing.Optional[PostV1CaptureDocumentsConfirmRequestNewSupplier]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
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

## Declarations
<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_intrastat_compute</a>(...) -> PostV1DeclarationsLtIntrastatComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_intrastat_compute(
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

**flow:** `PostV1DeclarationsLtIntrastatComputeRequestFlow` 
    
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

**transport_mode:** `typing.Optional[PostV1DeclarationsLtIntrastatComputeRequestTransportMode]` 
    
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_ivaz_generate</a>(...) -> PostV1DeclarationsLtIvazGenerateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_ivaz_generate(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_intrastat_obligation</a>(...) -> PostV1DeclarationsLtIntrastatObligationResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_intrastat_obligation(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_isaf_generate</a>(...) -> PostV1DeclarationsLtIsafGenerateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_isaf_generate(
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

**data_type:** `typing.Optional[PostV1DeclarationsLtIsafGenerateRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_fr0600compute</a>(...) -> PostV1DeclarationsLtFr0600ComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_fr0600compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_gpm313compute</a>(...) -> PostV1DeclarationsLtGpm313ComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_gpm313compute(
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

**payout_timing:** `typing.Optional[PostV1DeclarationsLtGpm313ComputeRequestPayoutTiming]` 
    
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_sam_compute</a>(...) -> PostV1DeclarationsLtSamComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_sam_compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_sd_generate</a>(...) -> PostV1DeclarationsLtSdGenerateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_sd_generate(
    type="1-SD",
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `PostV1DeclarationsLtSdGenerateRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_lt_saft_generate</a>(...) -> PostV1DeclarationsLtSaftGenerateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_lt_saft_generate(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**data_type:** `typing.Optional[PostV1DeclarationsLtSaftGenerateRequestDataType]` 
    
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_oss_compute</a>(...) -> PostV1DeclarationsEuOssComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_oss_compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_ioss_compute</a>(...) -> PostV1DeclarationsEuIossComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_ioss_compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_distance_sales_threshold_get</a>(...) -> PostV1DeclarationsEuDistanceSalesThresholdGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_distance_sales_threshold_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_union_turnover_get</a>(...) -> PostV1DeclarationsEuUnionTurnoverGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_union_turnover_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_sme_cross_border_report_compute</a>(...) -> PostV1DeclarationsEuSmeCrossBorderReportComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_sme_cross_border_report_compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_sme_thresholds_list</a>() -> PostV1DeclarationsEuSmeThresholdsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_sme_thresholds_list()

```
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_sme_threshold_get</a>(...) -> PostV1DeclarationsEuSmeThresholdGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_sme_threshold_get()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_vat_return_packs_list</a>() -> PostV1DeclarationsEuVatReturnPacksListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_vat_return_packs_list()

```
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_eu_vat_return_compute</a>(...) -> PostV1DeclarationsEuVatReturnComputeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_eu_vat_return_compute(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_pl_jpk_v7m_generate</a>(...) -> PostV1DeclarationsPlJpkV7MGenerateResponse</code></summary>
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

client.declarations.post_v1declarations_pl_jpk_v7m_generate(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_configs_list</a>() -> PostV1DeclarationsConfigsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_configs_list()

```
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_configs_update</a>(...) -> PostV1DeclarationsConfigsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_configs_update(
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_submissions_create</a>(...) -> PostV1DeclarationsSubmissionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_submissions_create(
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

**obligation:** `PostV1DeclarationsSubmissionsCreateRequestObligation` 
    
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

**data_type:** `typing.Optional[PostV1DeclarationsSubmissionsCreateRequestDataType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_submissions_mark</a>(...) -> PostV1DeclarationsSubmissionsMarkResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_submissions_mark(
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

**status:** `PostV1DeclarationsSubmissionsMarkRequestStatus` 
    
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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">post_v1declarations_submissions_list</a>(...) -> PostV1DeclarationsSubmissionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.declarations.post_v1declarations_submissions_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1DeclarationsSubmissionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1DeclarationsSubmissionsListRequestFilterItem]]` 
    
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

## Ledger
<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_accounts_list</a>(...) -> PostV1LedgerAccountsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_accounts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerAccountsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerAccountsListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_accounts_create</a>(...) -> PostV1LedgerAccountsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_accounts_create(
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

**type:** `PostV1LedgerAccountsCreateRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**translations:** `typing.Optional[PostV1LedgerAccountsCreateRequestTranslations]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_accounts_update</a>(...) -> PostV1LedgerAccountsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_accounts_update(
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

**translations:** `typing.Optional[PostV1LedgerAccountsUpdateRequestTranslations]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_accounts_apply_template</a>() -> PostV1LedgerAccountsApplyTemplateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_accounts_apply_template()

```
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_periods_list</a>(...) -> PostV1LedgerPeriodsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_periods_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerPeriodsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerPeriodsListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_periods_lock</a>(...) -> PostV1LedgerPeriodsLockResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_periods_lock(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_periods_unlock</a>(...) -> PostV1LedgerPeriodsUnlockResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_periods_unlock(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_journal_transactions_list</a>(...) -> PostV1LedgerJournalTransactionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_journal_transactions_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerJournalTransactionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerJournalTransactionsListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_centers_create</a>(...) -> PostV1LedgerCostCentersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_centers_create(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_centers_update</a>(...) -> PostV1LedgerCostCentersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_centers_update(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_centers_list</a>(...) -> PostV1LedgerCostCentersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_centers_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerCostCentersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerCostCentersListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_center_groups_create</a>(...) -> PostV1LedgerCostCenterGroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_center_groups_create(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_center_groups_update</a>(...) -> PostV1LedgerCostCenterGroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_center_groups_update(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_center_groups_delete</a>(...) -> PostV1LedgerCostCenterGroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_center_groups_delete(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_cost_center_groups_list</a>(...) -> PostV1LedgerCostCenterGroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_cost_center_groups_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerCostCenterGroupsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerCostCenterGroupsListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_posting_rules_list</a>() -> PostV1LedgerPostingRulesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_posting_rules_list()

```
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_posting_rules_update</a>(...) -> PostV1LedgerPostingRulesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.ledger import PostV1LedgerPostingRulesUpdateRequestRulesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_posting_rules_update(
    rules=[
        PostV1LedgerPostingRulesUpdateRequestRulesItem(
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

**rules:** `typing.List[PostV1LedgerPostingRulesUpdateRequestRulesItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_owners_create</a>(...) -> PostV1LedgerOwnersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_owners_create(
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

**shares_type:** `typing.Optional[PostV1LedgerOwnersCreateRequestSharesType]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_acquisition_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[PostV1LedgerOwnersCreateRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_owners_update</a>(...) -> PostV1LedgerOwnersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_owners_update(
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

**shares_type:** `typing.Optional[PostV1LedgerOwnersUpdateRequestSharesType]` 
    
</dd>
</dl>

<dl>
<dd>

**shares_acquisition_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**address:** `typing.Optional[PostV1LedgerOwnersUpdateRequestAddress]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_owners_delete</a>(...) -> PostV1LedgerOwnersDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_owners_delete(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_owners_list</a>(...) -> PostV1LedgerOwnersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_owners_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1LedgerOwnersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1LedgerOwnersListRequestFilterItem]]` 
    
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_journal_transactions_get</a>(...) -> PostV1LedgerJournalTransactionsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_journal_transactions_get(
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

<details><summary><code>client.ledger.<a href="src/nordlet/ledger/client.py">post_v1ledger_journal_transactions_create</a>(...) -> PostV1LedgerJournalTransactionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.ledger import PostV1LedgerJournalTransactionsCreateRequestEntriesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ledger.post_v1ledger_journal_transactions_create(
    date="date",
    entries=[
        PostV1LedgerJournalTransactionsCreateRequestEntriesItem(
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**entries:** `typing.List[PostV1LedgerJournalTransactionsCreateRequestEntriesItem]` 
    
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

## Migration
<details><summary><code>client.migration.<a href="src/nordlet/migration/client.py">check_a_historical_books_package_without_writing_anything</a>(...) -> PostV1MigrationBooksValidateResponse</code></summary>
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

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.migration.check_a_historical_books_package_without_writing_anything(
    cutover_date="cutoverDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cutover_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**source:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestAccountsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**partners:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestPartnersItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**opening_balances:** `typing.Optional[PostV1MigrationBooksValidateRequestOpeningBalances]` 
    
</dd>
</dl>

<dl>
<dd>

**journal:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestJournalItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_receivables:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestOpenReceivablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_payables:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestOpenPayablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**asset_groups:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestAssetGroupsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_assets:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestFixedAssetsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**stock:** `typing.Optional[typing.List[PostV1MigrationBooksValidateRequestStockItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.migration.<a href="src/nordlet/migration/client.py">import_historical_books_from_a_previous_accounting_system</a>(...) -> PostV1MigrationBooksImportResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Brings a company over from another system in one call: chart of accounts, partners, items, opening balances (or the full journal history), open customer and supplier invoices, fixed assets with their accumulated depreciation, and stock on hand. The whole package is written in one database transaction — if any row fails, nothing is stored.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.migration.import_historical_books_from_a_previous_accounting_system(
    cutover_date="cutoverDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**cutover_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**source:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**accounts:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestAccountsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**partners:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestPartnersItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**items:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**opening_balances:** `typing.Optional[PostV1MigrationBooksImportRequestOpeningBalances]` 
    
</dd>
</dl>

<dl>
<dd>

**journal:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestJournalItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_receivables:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestOpenReceivablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**open_payables:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestOpenPayablesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**asset_groups:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestAssetGroupsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**fixed_assets:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestFixedAssetsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**stock:** `typing.Optional[typing.List[PostV1MigrationBooksImportRequestStockItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Assets
<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_groups_create</a>(...) -> PostV1AssetsGroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_groups_create(
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_groups_list</a>(...) -> PostV1AssetsGroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_groups_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AssetsGroupsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AssetsGroupsListRequestFilterItem]]` 
    
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_assets_create</a>(...) -> PostV1AssetsAssetsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_assets_create(
    group_id="groupId",
    code="code",
    name="name",
    acquisition_date="acquisitionDate",
    acquisition_cost="acquisitionCost",
)

```
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

**acquisition_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_cost:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**depreciation_start_date:** `typing.Optional[str]` 
    
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

**documents:** `typing.Optional[typing.List[PostV1AssetsAssetsCreateRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_assets_get</a>(...) -> PostV1AssetsAssetsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_assets_get(
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_assets_list</a>(...) -> PostV1AssetsAssetsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_assets_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AssetsAssetsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AssetsAssetsListRequestFilterItem]]` 
    
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_assets_modernize</a>(...) -> PostV1AssetsAssetsModernizeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_assets_modernize(
    id="id",
    date="date",
    amount="amount",
)

```
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

**date:** `str` 
    
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_depreciation_preview</a>(...) -> PostV1AssetsDepreciationPreviewResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_depreciation_preview(
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

<details><summary><code>client.assets.<a href="src/nordlet/assets/client.py">post_v1assets_depreciation_post</a>(...) -> PostV1AssetsDepreciationPostResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.assets.post_v1assets_depreciation_post(
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

## Hr
<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_positions_create</a>(...) -> PostV1HrPositionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_positions_create(
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

**translations:** `typing.Optional[typing.Dict[str, PostV1HrPositionsCreateRequestTranslationsValue]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_positions_update</a>(...) -> PostV1HrPositionsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_positions_update(
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

**translations:** `typing.Optional[typing.Dict[str, typing.Optional[PostV1HrPositionsUpdateRequestTranslationsValue]]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_positions_list</a>(...) -> PostV1HrPositionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_positions_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1HrPositionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1HrPositionsListRequestFilterItem]]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_create</a>(...) -> PostV1HrEmployeesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_create(
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

**birth_date:** `typing.Optional[str]` 
    
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

**address:** `typing.Optional[PostV1HrEmployeesCreateRequestAddress]` 
    
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

**social_insurance_start:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**hire_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**apply_npd:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**npd_override:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pension_accumulation:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.List[PostV1HrEmployeesCreateRequestAttributesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_update</a>(...) -> PostV1HrEmployeesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_update(
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

**birth_date:** `typing.Optional[str]` 
    
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

**address:** `typing.Optional[PostV1HrEmployeesUpdateRequestAddress]` 
    
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

**social_insurance_start:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**hire_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**apply_npd:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**npd_override:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**pension_accumulation:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.List[PostV1HrEmployeesUpdateRequestAttributesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**termination_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PostV1HrEmployeesUpdateRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_get</a>(...) -> PostV1HrEmployeesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_get(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_list</a>(...) -> PostV1HrEmployeesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1HrEmployeesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1HrEmployeesListRequestFilterItem]]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_delete</a>(...) -> PostV1HrEmployeesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_delete(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">blank_an_employees_personal_data_and_hide_the_record</a>(...) -> PostV1HrEmployeesAnonymizeResponse</code></summary>
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

client.hr.blank_an_employees_personal_data_and_hide_the_record(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_contracts_create</a>(...) -> PostV1HrContractsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_contracts_create(
    employee_id="employeeId",
    start_date="startDate",
    base_salary="baseSalary",
)

```
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

**start_date:** `str` 
    
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

**type:** `typing.Optional[PostV1HrContractsCreateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**salary_type:** `typing.Optional[PostV1HrContractsCreateRequestSalaryType]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_contracts_end</a>(...) -> PostV1HrContractsEndResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_contracts_end(
    id="id",
    end_date="endDate",
)

```
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

**end_date:** `str` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_contracts_list</a>(...) -> PostV1HrContractsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_contracts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1HrContractsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1HrContractsListRequestFilterItem]]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_leave_balances_set</a>(...) -> PostV1HrLeaveBalancesSetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_leave_balances_set(
    employee_id="employeeId",
    year=1000000,
    entitled_days="entitledDays",
)

```
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_leave_balances_list</a>(...) -> PostV1HrLeaveBalancesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_leave_balances_list()

```
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_incapacity_certificates_create</a>(...) -> PostV1HrIncapacityCertificatesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_incapacity_certificates_create(
    employee_id="employeeId",
    number="number",
    from_date="fromDate",
    to_date="toDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_incapacity_certificates_list</a>(...) -> PostV1HrIncapacityCertificatesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_incapacity_certificates_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1HrIncapacityCertificatesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1HrIncapacityCertificatesListRequestFilterItem]]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_records_create</a>(...) -> PostV1HrEmployeesRecordsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_records_create(
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

**type:** `PostV1HrEmployeesRecordsCreateRequestType` 
    
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

**issued_at:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_until:** `typing.Optional[str]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_records_update</a>(...) -> PostV1HrEmployeesRecordsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_records_update(
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

**type:** `typing.Optional[PostV1HrEmployeesRecordsUpdateRequestType]` 
    
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

**issued_at:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**valid_until:** `typing.Optional[str]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_records_delete</a>(...) -> PostV1HrEmployeesRecordsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_records_delete(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_records_list</a>(...) -> PostV1HrEmployeesRecordsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_records_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1HrEmployeesRecordsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1HrEmployeesRecordsListRequestFilterItem]]` 
    
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_employees_attachments_list</a>(...) -> PostV1HrEmployeesAttachmentsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_employees_attachments_list(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_timesheets_generate</a>(...) -> PostV1HrTimesheetsGenerateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_timesheets_generate(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_timesheets_upsert</a>(...) -> PostV1HrTimesheetsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.hr import PostV1HrTimesheetsUpsertRequestDaysItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_timesheets_upsert(
    employee_id="employeeId",
    year=1000000,
    month=1000000,
    days=[
        PostV1HrTimesheetsUpsertRequestDaysItem(
            day=1000000,
            hours="hours",
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

**days:** `typing.List[PostV1HrTimesheetsUpsertRequestDaysItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_timesheets_get</a>(...) -> PostV1HrTimesheetsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_timesheets_get(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_timesheets_list</a>(...) -> PostV1HrTimesheetsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_timesheets_list(
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

<details><summary><code>client.hr.<a href="src/nordlet/hr/client.py">post_v1hr_timesheets_delete</a>(...) -> PostV1HrTimesheetsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.hr.post_v1hr_timesheets_delete(
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

## Fleet
<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_vehicles_create</a>(...) -> PostV1FleetVehiclesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_vehicles_create(
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

**fuel_type:** `typing.Optional[PostV1FleetVehiclesCreateRequestFuelType]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `typing.Optional[str]` 
    
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

**technical_inspection_due:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**insurance_due:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**notes:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**documents:** `typing.Optional[typing.List[PostV1FleetVehiclesCreateRequestDocumentsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_vehicles_update</a>(...) -> PostV1FleetVehiclesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_vehicles_update(
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

**fuel_type:** `typing.Optional[PostV1FleetVehiclesUpdateRequestFuelType]` 
    
</dd>
</dl>

<dl>
<dd>

**acquisition_date:** `typing.Optional[str]` 
    
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

**technical_inspection_due:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**insurance_due:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PostV1FleetVehiclesUpdateRequestStatus]` 
    
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

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_vehicles_get</a>(...) -> PostV1FleetVehiclesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_vehicles_get(
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

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_vehicles_list</a>(...) -> PostV1FleetVehiclesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_vehicles_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1FleetVehiclesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1FleetVehiclesListRequestFilterItem]]` 
    
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

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_assignments_create</a>(...) -> PostV1FleetAssignmentsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_assignments_create(
    vehicle_id="vehicleId",
    employee_id="employeeId",
    from_date="fromDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_assignments_end</a>(...) -> PostV1FleetAssignmentsEndResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_assignments_end(
    id="id",
    to_date="toDate",
)

```
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

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_assignments_list</a>(...) -> PostV1FleetAssignmentsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_assignments_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1FleetAssignmentsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1FleetAssignmentsListRequestFilterItem]]` 
    
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

<details><summary><code>client.fleet.<a href="src/nordlet/fleet/client.py">post_v1fleet_natura_preview</a>(...) -> PostV1FleetNaturaPreviewResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.fleet.post_v1fleet_natura_preview(
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

## Payroll
<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_departments_create</a>(...) -> PostV1PayrollDepartmentsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_departments_create(
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_departments_list</a>() -> PostV1PayrollDepartmentsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_departments_list()

```
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_schedules_create</a>(...) -> PostV1PayrollSchedulesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_schedules_create(
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_schedules_list</a>() -> PostV1PayrollSchedulesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_schedules_list()

```
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_calc</a>(...) -> PostV1PayrollCalcResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_calc(
    taxable_base="taxableBase",
    date="date",
)

```
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**apply_npd:** `typing.Optional[bool]` 
    
</dd>
</dl>

<dl>
<dd>

**npd_override:** `typing.Optional[str]` 
    
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_runs_create</a>(...) -> PostV1PayrollRunsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_runs_create(
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

**lines:** `typing.Optional[typing.List[PostV1PayrollRunsCreateRequestLinesItem]]` 
    
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_runs_get</a>(...) -> PostV1PayrollRunsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_runs_get(
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_runs_list</a>(...) -> PostV1PayrollRunsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_runs_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PayrollRunsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PayrollRunsListRequestFilterItem]]` 
    
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_runs_approve</a>(...) -> PostV1PayrollRunsApproveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_runs_approve(
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_runs_cancel</a>(...) -> PostV1PayrollRunsCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_runs_cancel(
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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">post_v1payroll_payments_export</a>(...) -> PostV1PayrollPaymentsExportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.payroll.post_v1payroll_payments_export(
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

**execution_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Agreements
<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_types_create</a>(...) -> PostV1AgreementsTypesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_types_create(
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_types_list</a>(...) -> PostV1AgreementsTypesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_types_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AgreementsTypesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AgreementsTypesListRequestFilterItem]]` 
    
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_create</a>(...) -> PostV1AgreementsAgreementsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_create(
    number="number",
    start_date="startDate",
)

```
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

**start_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type_id:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**kind:** `typing.Optional[PostV1AgreementsAgreementsCreateRequestKind]` 
    
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

**end_date:** `typing.Optional[str]` 
    
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

**billing_period:** `typing.Optional[PostV1AgreementsAgreementsCreateRequestBillingPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**currency:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PostV1AgreementsAgreementsCreateRequestStatus]` 
    
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

**items:** `typing.Optional[typing.List[PostV1AgreementsAgreementsCreateRequestItemsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_get</a>(...) -> PostV1AgreementsAgreementsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_get(
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_update</a>(...) -> PostV1AgreementsAgreementsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_update(
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

**kind:** `typing.Optional[PostV1AgreementsAgreementsUpdateRequestKind]` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**end_date:** `typing.Optional[str]` 
    
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

**billing_period:** `typing.Optional[PostV1AgreementsAgreementsUpdateRequestBillingPeriod]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[PostV1AgreementsAgreementsUpdateRequestStatus]` 
    
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_delete</a>(...) -> PostV1AgreementsAgreementsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_delete(
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_list</a>(...) -> PostV1AgreementsAgreementsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AgreementsAgreementsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AgreementsAgreementsListRequestFilterItem]]` 
    
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_generate_invoice</a>(...) -> PostV1AgreementsAgreementsGenerateInvoiceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_generate_invoice(
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

**as_of_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_agreements_billing_run</a>(...) -> PostV1AgreementsAgreementsBillingRunResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_agreements_billing_run()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_insurance_policies_create</a>(...) -> PostV1AgreementsInsurancePoliciesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_insurance_policies_create(
    policy_number="policyNumber",
    insured_object="insuredObject",
    from_date="fromDate",
    to_date="toDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_insurance_policies_list</a>(...) -> PostV1AgreementsInsurancePoliciesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_insurance_policies_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AgreementsInsurancePoliciesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AgreementsInsurancePoliciesListRequestFilterItem]]` 
    
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

<details><summary><code>client.agreements.<a href="src/nordlet/agreements/client.py">post_v1agreements_insurance_policies_delete</a>(...) -> PostV1AgreementsInsurancePoliciesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.agreements.post_v1agreements_insurance_policies_delete(
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

## Inventory
<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_settings_get</a>() -> PostV1InventorySettingsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_settings_get()

```
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_settings_update</a>(...) -> PostV1InventorySettingsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_settings_update(
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

**negative_stock_policy:** `PostV1InventorySettingsUpdateRequestNegativeStockPolicy` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_warehouses_create</a>(...) -> PostV1InventoryWarehousesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_warehouses_create(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_warehouses_list</a>(...) -> PostV1InventoryWarehousesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_warehouses_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1InventoryWarehousesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1InventoryWarehousesListRequestFilterItem]]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_receive</a>(...) -> PostV1InventoryStockReceiveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_receive(
    warehouse_id="warehouseId",
    item_id="itemId",
    date="date",
    quantity="quantity",
    unit_cost="unitCost",
)

```
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

**date:** `str` 
    
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

**expiry_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_write_off</a>(...) -> PostV1InventoryStockWriteOffResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_write_off(
    warehouse_id="warehouseId",
    item_id="itemId",
    date="date",
    quantity="quantity",
)

```
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

**date:** `str` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_transfer</a>(...) -> PostV1InventoryStockTransferResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_transfer(
    from_warehouse_id="fromWarehouseId",
    to_warehouse_id="toWarehouseId",
    item_id="itemId",
    date="date",
    quantity="quantity",
)

```
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

**date:** `str` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_take</a>(...) -> PostV1InventoryStockTakeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.inventory import PostV1InventoryStockTakeRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_take(
    warehouse_id="warehouseId",
    date="date",
    lines=[
        PostV1InventoryStockTakeRequestLinesItem(
            counted_qty="countedQty",
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**lines:** `typing.List[PostV1InventoryStockTakeRequestLinesItem]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_levels</a>(...) -> PostV1InventoryStockLevelsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_levels()

```
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_stock_movements_list</a>(...) -> PostV1InventoryStockMovementsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_stock_movements_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1InventoryStockMovementsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1InventoryStockMovementsListRequestFilterItem]]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_lots_list</a>(...) -> PostV1InventoryLotsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_lots_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1InventoryLotsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1InventoryLotsListRequestFilterItem]]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_lots_get</a>(...) -> PostV1InventoryLotsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_lots_get(
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_lots_update</a>(...) -> PostV1InventoryLotsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_lots_update(
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

**expiry_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_landed_costs_create</a>(...) -> PostV1InventoryLandedCostsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_landed_costs_create(
    date="date",
    amount="amount",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**method:** `typing.Optional[PostV1InventoryLandedCostsCreateRequestMethod]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_landed_costs_get</a>(...) -> PostV1InventoryLandedCostsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_landed_costs_get(
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_landed_costs_list</a>(...) -> PostV1InventoryLandedCostsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_landed_costs_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1InventoryLandedCostsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1InventoryLandedCostsListRequestFilterItem]]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_reorder_rules_create</a>(...) -> PostV1InventoryReorderRulesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_reorder_rules_create(
    item_id="itemId",
    min_qty="minQty",
)

```
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_reorder_rules_update</a>(...) -> PostV1InventoryReorderRulesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_reorder_rules_update(
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_reorder_rules_delete</a>(...) -> PostV1InventoryReorderRulesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_reorder_rules_delete(
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_reorder_rules_list</a>(...) -> PostV1InventoryReorderRulesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_reorder_rules_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1InventoryReorderRulesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1InventoryReorderRulesListRequestFilterItem]]` 
    
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

<details><summary><code>client.inventory.<a href="src/nordlet/inventory/client.py">post_v1inventory_reorder_rules_check</a>() -> PostV1InventoryReorderRulesCheckResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.inventory.post_v1inventory_reorder_rules_check()

```
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

## Production
<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_work_centers_create</a>(...) -> PostV1ProductionWorkCentersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_work_centers_create(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_work_centers_update</a>(...) -> PostV1ProductionWorkCentersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_work_centers_update(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_work_centers_list</a>(...) -> PostV1ProductionWorkCentersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_work_centers_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionWorkCentersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionWorkCentersListRequestFilterItem]]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_routings_create</a>(...) -> PostV1ProductionRoutingsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.production import PostV1ProductionRoutingsCreateRequestOperationsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_routings_create(
    code="code",
    name="name",
    operations=[
        PostV1ProductionRoutingsCreateRequestOperationsItem(
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

**operations:** `typing.List[PostV1ProductionRoutingsCreateRequestOperationsItem]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_routings_get</a>(...) -> PostV1ProductionRoutingsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_routings_get(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_routings_list</a>(...) -> PostV1ProductionRoutingsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_routings_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionRoutingsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionRoutingsListRequestFilterItem]]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_maintenance_create</a>(...) -> PostV1ProductionMaintenanceCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_maintenance_create(
    work_center_id="workCenterId",
    type="preventive",
    planned_date="plannedDate",
)

```
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

**type:** `PostV1ProductionMaintenanceCreateRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**planned_date:** `str` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_maintenance_complete</a>(...) -> PostV1ProductionMaintenanceCompleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_maintenance_complete(
    id="id",
    completed_date="completedDate",
)

```
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

**completed_date:** `str` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_maintenance_cancel</a>(...) -> PostV1ProductionMaintenanceCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_maintenance_cancel(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_maintenance_list</a>(...) -> PostV1ProductionMaintenanceListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_maintenance_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionMaintenanceListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionMaintenanceListRequestFilterItem]]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_boms_create</a>(...) -> PostV1ProductionBomsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.production import PostV1ProductionBomsCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_boms_create(
    code="code",
    name="name",
    finished_item_id="finishedItemId",
    lines=[
        PostV1ProductionBomsCreateRequestLinesItem(
            component_item_id="componentItemId",
            quantity="quantity",
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

**lines:** `typing.List[PostV1ProductionBomsCreateRequestLinesItem]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_boms_get</a>(...) -> PostV1ProductionBomsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_boms_get(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_boms_list</a>(...) -> PostV1ProductionBomsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_boms_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionBomsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionBomsListRequestFilterItem]]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_orders_create</a>(...) -> PostV1ProductionOrdersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_orders_create(
    bom_id="bomId",
    warehouse_id="warehouseId",
    quantity="quantity",
    date="date",
)

```
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[PostV1ProductionOrdersCreateRequestType]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_orders_record_operation</a>(...) -> PostV1ProductionOrdersRecordOperationResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_orders_record_operation(
    id="id",
    actual_minutes="actualMinutes",
)

```
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_quality_checks_add</a>(...) -> PostV1ProductionQualityChecksAddResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_quality_checks_add(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_quality_checks_record</a>(...) -> PostV1ProductionQualityChecksRecordResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_quality_checks_record(
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

**result:** `PostV1ProductionQualityChecksRecordRequestResult` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_quality_checks_list</a>(...) -> PostV1ProductionQualityChecksListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_quality_checks_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionQualityChecksListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionQualityChecksListRequestFilterItem]]` 
    
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_orders_complete</a>(...) -> PostV1ProductionOrdersCompleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_orders_complete(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_orders_get</a>(...) -> PostV1ProductionOrdersGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_orders_get(
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

<details><summary><code>client.production.<a href="src/nordlet/production/client.py">post_v1production_orders_list</a>(...) -> PostV1ProductionOrdersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.production.post_v1production_orders_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProductionOrdersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProductionOrdersListRequestFilterItem]]` 
    
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

## Ecommerce
<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_create</a>(...) -> PostV1EcommerceOrdersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.ecommerce import PostV1EcommerceOrdersCreateRequestLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_create(
    lines=[
        PostV1EcommerceOrdersCreateRequestLinesItem(
            description="description",
            quantity="quantity",
            unit_price_excl_vat="unitPriceExclVat",
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

**lines:** `typing.List[PostV1EcommerceOrdersCreateRequestLinesItem]` 
    
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

**partner:** `typing.Optional[PostV1EcommerceOrdersCreateRequestPartner]` 
    
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_get</a>(...) -> PostV1EcommerceOrdersGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_get(
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_list</a>(...) -> PostV1EcommerceOrdersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1EcommerceOrdersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1EcommerceOrdersListRequestFilterItem]]` 
    
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_reserve</a>(...) -> PostV1EcommerceOrdersReserveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_reserve(
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_fulfill</a>(...) -> PostV1EcommerceOrdersFulfillResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_fulfill(
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

**date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_orders_cancel</a>(...) -> PostV1EcommerceOrdersCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_orders_cancel(
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_products_list</a>(...) -> PostV1EcommerceProductsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_products_list()

```
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

<details><summary><code>client.ecommerce.<a href="src/nordlet/ecommerce/client.py">post_v1ecommerce_stock_list</a>(...) -> PostV1EcommerceStockListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.ecommerce.post_v1ecommerce_stock_list()

```
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

## Cash
<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">post_v1cash_orders_create</a>(...) -> PostV1CashOrdersCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.post_v1cash_orders_create(
    type="receipt",
    date="date",
    amount="amount",
    purpose="purpose",
    counter_account_code="counterAccountCode",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**type:** `PostV1CashOrdersCreateRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**date:** `str` 
    
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

**counter_account_code:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**cash_account_code:** `typing.Optional[str]` 
    
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

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">post_v1cash_orders_get</a>(...) -> PostV1CashOrdersGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.post_v1cash_orders_get(
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

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">post_v1cash_orders_list</a>(...) -> PostV1CashOrdersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.post_v1cash_orders_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1CashOrdersListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1CashOrdersListRequestFilterItem]]` 
    
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

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">post_v1cash_balance</a>(...) -> PostV1CashBalanceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.post_v1cash_balance()

```
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

**as_of:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.cash.<a href="src/nordlet/cash/client.py">post_v1cash_advance_holders_balances</a>() -> PostV1CashAdvanceHoldersBalancesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.cash.post_v1cash_advance_holders_balances()

```
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

## Projects
<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_create</a>(...) -> PostV1ProjectsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_create(
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_update</a>(...) -> PostV1ProjectsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_update(
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

**status:** `typing.Optional[PostV1ProjectsUpdateRequestStatus]` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_get</a>(...) -> PostV1ProjectsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_get(
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_list</a>(...) -> PostV1ProjectsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProjectsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProjectsListRequestFilterItem]]` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_time_entries_create</a>(...) -> PostV1ProjectsTimeEntriesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_time_entries_create(
    project_id="projectId",
    date="date",
    hours="hours",
)

```
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

**date:** `str` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_time_entries_update</a>(...) -> PostV1ProjectsTimeEntriesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_time_entries_update(
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

**date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_time_entries_delete</a>(...) -> PostV1ProjectsTimeEntriesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_time_entries_delete(
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_time_entries_list</a>(...) -> PostV1ProjectsTimeEntriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_time_entries_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ProjectsTimeEntriesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ProjectsTimeEntriesListRequestFilterItem]]` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_time_entries_bill</a>(...) -> PostV1ProjectsTimeEntriesBillResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_time_entries_bill(
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

**date_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[str]` 
    
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

**issue_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**due_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**group_by:** `typing.Optional[PostV1ProjectsTimeEntriesBillRequestGroupBy]` 
    
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

<details><summary><code>client.projects.<a href="src/nordlet/projects/client.py">post_v1projects_report</a>(...) -> PostV1ProjectsReportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.projects.post_v1projects_report()

```
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

**date_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Transport
<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_create</a>(...) -> PostV1TransportWaybillsCreateResponse</code></summary>
<dl>
<dd>

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

client.transport.post_v1transport_waybills_create(
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

**document_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1TransportWaybillsCreateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_update</a>(...) -> PostV1TransportWaybillsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.post_v1transport_waybills_update(
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

**document_date:** `typing.Optional[str]` 
    
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

**lines:** `typing.Optional[typing.List[PostV1TransportWaybillsUpdateRequestLinesItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_issue</a>(...) -> PostV1TransportWaybillsIssueResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.post_v1transport_waybills_issue(
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

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_cancel</a>(...) -> PostV1TransportWaybillsCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.post_v1transport_waybills_cancel(
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

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_get</a>(...) -> PostV1TransportWaybillsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.post_v1transport_waybills_get(
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

<details><summary><code>client.transport.<a href="src/nordlet/transport/client.py">post_v1transport_waybills_list</a>(...) -> PostV1TransportWaybillsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.transport.post_v1transport_waybills_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1TransportWaybillsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1TransportWaybillsListRequestFilterItem]]` 
    
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

## Pos
<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_devices_create</a>(...) -> PostV1PosDevicesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_devices_create(
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

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_devices_update</a>(...) -> PostV1PosDevicesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_devices_update(
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

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_devices_list</a>(...) -> PostV1PosDevicesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_devices_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PosDevicesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PosDevicesListRequestFilterItem]]` 
    
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

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_reports_create</a>(...) -> PostV1PosReportsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.pos import PostV1PosReportsCreateRequestVatLinesItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_reports_create(
    report_number="reportNumber",
    date="date",
    vat_lines=[
        PostV1PosReportsCreateRequestVatLinesItem(
            vat_rate_percent="vatRatePercent",
            net_amount="netAmount",
            vat_amount="vatAmount",
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**vat_lines:** `typing.List[PostV1PosReportsCreateRequestVatLinesItem]` 
    
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

**item_lines:** `typing.Optional[typing.List[PostV1PosReportsCreateRequestItemLinesItem]]` 
    
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

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_reports_get</a>(...) -> PostV1PosReportsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_reports_get(
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

<details><summary><code>client.pos.<a href="src/nordlet/pos/client.py">post_v1pos_reports_list</a>(...) -> PostV1PosReportsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.pos.post_v1pos_reports_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1PosReportsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1PosReportsListRequestFilterItem]]` 
    
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

## Calendar
<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">post_v1calendar_list</a>(...) -> PostV1CalendarListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.post_v1calendar_list()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `typing.Optional[str]` 
    
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

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">post_v1calendar_get</a>(...) -> PostV1CalendarGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.post_v1calendar_get(
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

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">post_v1calendar_create</a>(...) -> PostV1CalendarCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.post_v1calendar_create(
    title="title",
    due_date="dueDate",
)

```
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

**due_date:** `str` 
    
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

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">post_v1calendar_update</a>(...) -> PostV1CalendarUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.post_v1calendar_update(
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

**due_date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.calendar.<a href="src/nordlet/calendar/client.py">post_v1calendar_delete</a>(...) -> PostV1CalendarDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.calendar.post_v1calendar_delete(
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

## Audit
<details><summary><code>client.audit.<a href="src/nordlet/audit/client.py">post_v1audit_list</a>(...) -> PostV1AuditListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.audit.post_v1audit_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1AuditListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1AuditListRequestFilterItem]]` 
    
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

## Webhooks
<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_subscriptions_create</a>(...) -> PostV1WebhooksSubscriptionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_subscriptions_create(
    url="url",
    events=[
        "events"
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

**events:** `typing.List[str]` 
    
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

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_subscriptions_list</a>(...) -> PostV1WebhooksSubscriptionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_subscriptions_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1WebhooksSubscriptionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1WebhooksSubscriptionsListRequestFilterItem]]` 
    
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

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_subscriptions_update</a>(...) -> PostV1WebhooksSubscriptionsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_subscriptions_update(
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

**events:** `typing.Optional[typing.List[str]]` 
    
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

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_subscriptions_delete</a>(...) -> PostV1WebhooksSubscriptionsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_subscriptions_delete(
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

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_deliveries_list</a>(...) -> PostV1WebhooksDeliveriesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_deliveries_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1WebhooksDeliveriesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1WebhooksDeliveriesListRequestFilterItem]]` 
    
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

<details><summary><code>client.webhooks.<a href="src/nordlet/webhooks/client.py">post_v1webhooks_deliveries_redeliver</a>(...) -> PostV1WebhooksDeliveriesRedeliverResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.webhooks.post_v1webhooks_deliveries_redeliver(
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

## Bank
<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_accounts_create</a>(...) -> PostV1BankAccountsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_accounts_create(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_accounts_list</a>(...) -> PostV1BankAccountsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_accounts_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankAccountsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankAccountsListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_accounts_update</a>(...) -> PostV1BankAccountsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_accounts_update(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_transactions_import</a>(...) -> PostV1BankTransactionsImportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment
from nordlet.bank import PostV1BankTransactionsImportRequestTransactionsItem

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_transactions_import(
    bank_account_id="bankAccountId",
    transactions=[
        PostV1BankTransactionsImportRequestTransactionsItem(
            date="date",
            amount="amount",
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

**transactions:** `typing.List[PostV1BankTransactionsImportRequestTransactionsItem]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_statements_import</a>(...) -> PostV1BankStatementsImportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_statements_import(
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

**format:** `typing.Optional[PostV1BankStatementsImportRequestFormat]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_transactions_list</a>(...) -> PostV1BankTransactionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_transactions_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankTransactionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankTransactionsListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_transactions_match</a>(...) -> PostV1BankTransactionsMatchResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_transactions_match(
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

**document_type:** `PostV1BankTransactionsMatchRequestDocumentType` 
    
</dd>
</dl>

<dl>
<dd>

**document_id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_transactions_record</a>(...) -> PostV1BankTransactionsRecordResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_transactions_record(
    bank_account_id="bankAccountId",
    date="date",
    amount="amount",
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

**date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**amount:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**document_type:** `PostV1BankTransactionsRecordRequestDocumentType` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_payments_export</a>(...) -> PostV1BankPaymentsExportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_payments_export(
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

**execution_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">create_a_bank_import_template_fields_default_to_the_types_standard_field_list</a>(...) -> PostV1BankImportTemplatesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.create_a_bank_import_template_fields_default_to_the_types_standard_field_list(
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

**type:** `PostV1BankImportTemplatesCreateRequestType` 
    
</dd>
</dl>

<dl>
<dd>

**fields:** `typing.Optional[typing.List[PostV1BankImportTemplatesCreateRequestFieldsItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_import_templates_update</a>(...) -> PostV1BankImportTemplatesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_import_templates_update(
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

**type:** `typing.Optional[PostV1BankImportTemplatesUpdateRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**fields:** `typing.Optional[typing.List[PostV1BankImportTemplatesUpdateRequestFieldsItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_import_templates_delete</a>(...) -> PostV1BankImportTemplatesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_import_templates_delete(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_import_templates_get</a>(...) -> PostV1BankImportTemplatesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_import_templates_get(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_import_templates_list</a>(...) -> PostV1BankImportTemplatesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_import_templates_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankImportTemplatesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankImportTemplatesListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_match_rules_create</a>(...) -> PostV1BankMatchRulesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_match_rules_create(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_match_rules_update</a>(...) -> PostV1BankMatchRulesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_match_rules_update(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_match_rules_delete</a>(...) -> PostV1BankMatchRulesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_match_rules_delete(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_match_rules_list</a>() -> PostV1BankMatchRulesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_match_rules_list()

```
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_mandates_create</a>(...) -> PostV1BankMandatesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_mandates_create(
    partner_id="partnerId",
    iban="iban",
    signature_date="signatureDate",
)

```
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

**signature_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**bic:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**scheme:** `typing.Optional[PostV1BankMandatesCreateRequestScheme]` 
    
</dd>
</dl>

<dl>
<dd>

**sequence_type:** `typing.Optional[PostV1BankMandatesCreateRequestSequenceType]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_mandates_update</a>(...) -> PostV1BankMandatesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_mandates_update(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_mandates_cancel</a>(...) -> PostV1BankMandatesCancelResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_mandates_cancel(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_mandates_get</a>(...) -> PostV1BankMandatesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_mandates_get(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_mandates_list</a>(...) -> PostV1BankMandatesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_mandates_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankMandatesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankMandatesListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_direct_debits_export</a>(...) -> PostV1BankDirectDebitsExportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_direct_debits_export(
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

**collection_date:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_transactions_suggest_matches</a>(...) -> PostV1BankTransactionsSuggestMatchesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_transactions_suggest_matches(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_import</a>(...) -> PostV1BankSettlementsImportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_settlements_import(
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

**provider:** `typing.Optional[PostV1BankSettlementsImportRequestProvider]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_list</a>(...) -> PostV1BankSettlementsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_settlements_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankSettlementsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankSettlementsListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_get</a>(...) -> PostV1BankSettlementsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_settlements_get(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_match</a>(...) -> PostV1BankSettlementsMatchResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_settlements_match(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_link</a>(...) -> PostV1BankSettlementsLinkResponse</code></summary>
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

client.bank.post_v1bank_settlements_link(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_unlink</a>(...) -> PostV1BankSettlementsUnlinkResponse</code></summary>
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

client.bank.post_v1bank_settlements_unlink(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_settlements_post</a>(...) -> PostV1BankSettlementsPostResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_settlements_post(
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

**date:** `typing.Optional[str]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">list_the_psd2banks_asps_ps_available_to_connect</a>(...) -> PostV1BankFeedsBanksListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.list_the_psd2banks_asps_ps_available_to_connect()

```
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">begin_bank_authorization_redirect_the_user_to_the_returned_url</a>(...) -> PostV1BankFeedsConnectionsStartResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.begin_bank_authorization_redirect_the_user_to_the_returned_url(
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

**psu_type:** `typing.Optional[PostV1BankFeedsConnectionsStartRequestPsuType]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">exchange_the_redirect_code_for_a_session_and_store_the_bank_accounts_it_exposes</a>(...) -> PostV1BankFeedsConnectionsCompleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.exchange_the_redirect_code_for_a_session_and_store_the_bank_accounts_it_exposes(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_feeds_connections_get</a>(...) -> PostV1BankFeedsConnectionsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_feeds_connections_get(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">post_v1bank_feeds_connections_list</a>(...) -> PostV1BankFeedsConnectionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.post_v1bank_feeds_connections_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1BankFeedsConnectionsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1BankFeedsConnectionsListRequestFilterItem]]` 
    
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">revoke_the_consent_at_the_bank_and_drop_the_stored_connection</a>(...) -> PostV1BankFeedsConnectionsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.revoke_the_consent_at_the_bank_and_drop_the_stored_connection(
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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">point_a_bank_feed_account_at_a_ledger_bank_account_so_its_transactions_can_be_synced</a>(...) -> PostV1BankFeedsAccountsLinkResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.point_a_bank_feed_account_at_a_ledger_bank_account_so_its_transactions_can_be_synced(
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

**create_bank_account:** `typing.Optional[PostV1BankFeedsAccountsLinkRequestCreateBankAccount]` 
    
</dd>
</dl>

<dl>
<dd>

**sync_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">choose_the_import_template_applied_on_sync_and_how_often_the_account_is_synced_automatically</a>(...) -> PostV1BankFeedsAccountsConfigureResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.choose_the_import_template_applied_on_sync_and_how_often_the_account_is_synced_automatically(
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

**sync_schedule:** `typing.Optional[PostV1BankFeedsAccountsConfigureRequestSyncSchedule]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">pull_new_transactions_from_the_bank_into_the_ledger_emits_bank_feed_synced</a>(...) -> PostV1BankFeedsSyncResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.bank.pull_new_transactions_from_the_bank_into_the_ledger_emits_bank_feed_synced(
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

**date_from:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**date_to:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Files
<details><summary><code>client.files.<a href="src/nordlet/files/client.py">post_v1files_upload</a>(...) -> PostV1FilesUploadResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.post_v1files_upload(
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

**mime_type:** `str` 
    
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

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">post_v1files_get</a>(...) -> PostV1FilesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.post_v1files_get(
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

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">post_v1files_list</a>(...) -> PostV1FilesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.post_v1files_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1FilesListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1FilesListRequestFilterItem]]` 
    
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

<details><summary><code>client.files.<a href="src/nordlet/files/client.py">post_v1files_delete</a>(...) -> PostV1FilesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.files.post_v1files_delete(
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

## Reports
<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_trial_balance</a>(...) -> PostV1ReportsTrialBalanceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_trial_balance(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_size_category</a>(...) -> PostV1ReportsSizeCategoryResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_size_category(
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_financial_statements</a>(...) -> PostV1ReportsFinancialStatementsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_financial_statements(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[PostV1ReportsFinancialStatementsRequestCategory]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_general_journal</a>(...) -> PostV1ReportsGeneralJournalResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_general_journal(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_gl_detail</a>(...) -> PostV1ReportsGlDetailResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_gl_detail(
    account_code="accountCode",
    from_date="fromDate",
    to_date="toDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_partner_balances</a>() -> PostV1ReportsPartnerBalancesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_partner_balances()

```
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_debt_aging</a>(...) -> PostV1ReportsDebtAgingResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_debt_aging()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**side:** `typing.Optional[PostV1ReportsDebtAgingRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**as_of:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_monthly_summary</a>(...) -> PostV1ReportsMonthlySummaryResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_monthly_summary()

```
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_stock_balance</a>(...) -> PostV1ReportsStockBalanceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_stock_balance(
    as_of="asOf",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_stock_movement</a>(...) -> PostV1ReportsStockMovementResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_stock_movement(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_vat_summary</a>(...) -> PostV1ReportsVatSummaryResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_vat_summary(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**side:** `typing.Optional[PostV1ReportsVatSummaryRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_cash_flow</a>(...) -> PostV1ReportsCashFlowResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_cash_flow(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_stock_aging</a>(...) -> PostV1ReportsStockAgingResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_stock_aging(
    as_of="asOf",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**as_of:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_stock_shortage</a>(...) -> PostV1ReportsStockShortageResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_stock_shortage()

```
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_eu_purchases</a>(...) -> PostV1ReportsEuPurchasesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_eu_purchases(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_vat_detail</a>(...) -> PostV1ReportsVatDetailResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_vat_detail(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**side:** `typing.Optional[PostV1ReportsVatDetailRequestSide]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_pos_sales</a>(...) -> PostV1ReportsPosSalesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_pos_sales(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_online_sales</a>(...) -> PostV1ReportsOnlineSalesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_online_sales(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_oss</a>(...) -> PostV1ReportsOssResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_oss(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_advance_reconciliation</a>(...) -> PostV1ReportsAdvanceReconciliationResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_advance_reconciliation(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_write_off_acts</a>(...) -> PostV1ReportsWriteOffActsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_write_off_acts(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_cost_centers</a>(...) -> PostV1ReportsCostCentersResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_cost_centers(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_cost_center_activity</a>(...) -> PostV1ReportsCostCenterActivityResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_cost_center_activity(
    from_date="fromDate",
    to_date="toDate",
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_cost_center_items</a>(...) -> PostV1ReportsCostCenterItemsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_cost_center_items(
    from_date="fromDate",
    to_date="toDate",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_jobs_create</a>(...) -> PostV1ReportsJobsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_jobs_create(
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

**formats:** `typing.Optional[typing.List[PostV1ReportsJobsCreateRequestFormatsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_jobs_get</a>(...) -> PostV1ReportsJobsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_jobs_get(
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

<details><summary><code>client.reports.<a href="src/nordlet/reports/client.py">post_v1reports_jobs_list</a>(...) -> PostV1ReportsJobsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.reports.post_v1reports_jobs_list()

```
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

**sort:** `typing.Optional[typing.List[PostV1ReportsJobsListRequestSortItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `typing.Optional[typing.List[PostV1ReportsJobsListRequestFilterItem]]` 
    
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

## Consolidation
<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_groups_create</a>(...) -> PostV1ConsolidationGroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_groups_create(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_groups_list</a>() -> PostV1ConsolidationGroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_groups_list()

```
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_groups_get</a>(...) -> PostV1ConsolidationGroupsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_groups_get(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_groups_update</a>(...) -> PostV1ConsolidationGroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_groups_update(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_groups_delete</a>(...) -> PostV1ConsolidationGroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_groups_delete(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_members_add</a>(...) -> PostV1ConsolidationMembersAddResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_members_add(
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

**method:** `typing.Optional[PostV1ConsolidationMembersAddRequestMethod]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_members_remove</a>(...) -> PostV1ConsolidationMembersRemoveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_members_remove(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_intercompany_candidates</a>(...) -> PostV1ConsolidationIntercompanyCandidatesResponse</code></summary>
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

client.consolidation.post_v1consolidation_intercompany_candidates(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_intercompany_links_set</a>(...) -> PostV1ConsolidationIntercompanyLinksSetResponse</code></summary>
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

client.consolidation.post_v1consolidation_intercompany_links_set(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_intercompany_links_list</a>(...) -> PostV1ConsolidationIntercompanyLinksListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_intercompany_links_list(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_intercompany_links_remove</a>(...) -> PostV1ConsolidationIntercompanyLinksRemoveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_intercompany_links_remove(
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

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_intercompany_report</a>(...) -> PostV1ConsolidationIntercompanyReportResponse</code></summary>
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

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_intercompany_report(
    group_id="groupId",
    from_date="fromDate",
    to_date="toDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consolidation.<a href="src/nordlet/consolidation/client.py">post_v1consolidation_report</a>(...) -> PostV1ConsolidationReportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.consolidation.post_v1consolidation_report(
    group_id="groupId",
    from_date="fromDate",
    to_date="toDate",
)

```
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

**from_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to_date:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[PostV1ConsolidationReportRequestCategory]` 
    
</dd>
</dl>

<dl>
<dd>

**eliminations:** `typing.Optional[typing.List[PostV1ConsolidationReportRequestEliminationsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Public
<details><summary><code>client.public.<a href="src/nordlet/public/client.py">post_v1public_integration_requests</a>(...) -> PostV1PublicIntegrationRequestsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.public.post_v1public_integration_requests(
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

<details><summary><code>client.public.<a href="src/nordlet/public/client.py">get_v1public_pay_token</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.public.get_v1public_pay_token(
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

## Billing
<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_account_get</a>() -> PostV1BillingAccountGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_account_get()

```
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

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_account_set_plan</a>(...) -> PostV1BillingAccountSetPlanResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_account_set_plan(
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

**plan:** `PostV1BillingAccountSetPlanRequestPlan` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_topup_create</a>(...) -> PostV1BillingTopupCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_topup_create(
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

**locale:** `typing.Optional[PostV1BillingTopupCreateRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_portal_create</a>(...) -> PostV1BillingPortalCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_portal_create()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `typing.Optional[PostV1BillingPortalCreateRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_transactions_list</a>(...) -> PostV1BillingTransactionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_transactions_list()

```
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

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">post_v1billing_usage_list</a>(...) -> PostV1BillingUsageListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.billing.post_v1billing_usage_list(
    from_="from",
    to="to",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**from:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**to:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Account
<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_login_link_request</a>(...) -> PostV1AccountLoginLinkRequestResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_login_link_request(
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

**locale:** `typing.Optional[PostV1AccountLoginLinkRequestRequestLocale]` 
    
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_login_link_consume</a>(...) -> PostV1AccountLoginLinkConsumeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_login_link_consume(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_logout</a>() -> PostV1AccountLogoutResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_logout()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_me</a>() -> PostV1AccountMeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_me()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_members_list</a>() -> PostV1AccountMembersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_members_list()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_members_set_role</a>(...) -> PostV1AccountMembersSetRoleResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_members_set_role(
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

**role:** `PostV1AccountMembersSetRoleRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_members_remove</a>(...) -> PostV1AccountMembersRemoveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_members_remove(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_invites_create</a>(...) -> PostV1AccountInvitesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_invites_create(
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

**role:** `PostV1AccountInvitesCreateRequestRole` 
    
</dd>
</dl>

<dl>
<dd>

**locale:** `typing.Optional[PostV1AccountInvitesCreateRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_invites_list</a>() -> PostV1AccountInvitesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_invites_list()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_invites_revoke</a>(...) -> PostV1AccountInvitesRevokeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_invites_revoke(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_invites_get</a>(...) -> PostV1AccountInvitesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_invites_get(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_invites_accept</a>(...) -> PostV1AccountInvitesAcceptResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_invites_accept(
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

**locale:** `typing.Optional[PostV1AccountInvitesAcceptRequestLocale]` 
    
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_locale_set</a>(...) -> PostV1AccountLocaleSetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_locale_set(
    locale="lt",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**locale:** `PostV1AccountLocaleSetRequestLocale` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_create</a>(...) -> PostV1AccountCompaniesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_create(
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

**address:** `typing.Optional[PostV1AccountCompaniesCreateRequestAddress]` 
    
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

**country_code:** `typing.Optional[PostV1AccountCompaniesCreateRequestCountryCode]` — Jurisdiction the company is registered in (immutable after creation)
    
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_select</a>(...) -> PostV1AccountCompaniesSelectResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_select(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_profile</a>() -> PostV1AccountCompaniesProfileResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_profile()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_update</a>(...) -> PostV1AccountCompaniesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_update()

```
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

**address:** `typing.Optional[PostV1AccountCompaniesUpdateRequestAddress]` 
    
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

**logo:** `typing.Optional[PostV1AccountCompaniesUpdateRequestLogo]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_archive</a>(...) -> PostV1AccountCompaniesArchiveResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_archive(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_delete</a>(...) -> PostV1AccountCompaniesDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_delete(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_companies_activate</a>(...) -> PostV1AccountCompaniesActivateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_companies_activate(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_api_keys_create</a>(...) -> PostV1AccountApiKeysCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_api_keys_create(
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

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_api_keys_list</a>() -> PostV1AccountApiKeysListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_api_keys_list()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_api_keys_revoke</a>(...) -> PostV1AccountApiKeysRevokeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_api_keys_revoke(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_consent_accept</a>(...) -> PostV1AccountConsentAcceptResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_consent_accept(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_profile_update</a>(...) -> PostV1AccountProfileUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_profile_update()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_email_change_request</a>(...) -> PostV1AccountEmailChangeRequestResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_email_change_request(
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

**locale:** `typing.Optional[PostV1AccountEmailChangeRequestRequestLocale]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_sessions_list</a>() -> PostV1AccountSessionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_sessions_list()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_sessions_revoke</a>(...) -> PostV1AccountSessionsRevokeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_sessions_revoke(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_sessions_revoke_others</a>() -> PostV1AccountSessionsRevokeOthersResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_sessions_revoke_others()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">download_everything_nordlet_stores_about_the_signed_in_user</a>() -> PostV1AccountExportResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.download_everything_nordlet_stores_about_the_signed_in_user()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">delete_the_signed_in_user_account</a>(...) -> PostV1AccountDeleteResponse</code></summary>
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

client.account.delete_the_signed_in_user_account(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_referral_get</a>() -> PostV1AccountReferralGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_referral_get()

```
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_table_settings_get</a>(...) -> PostV1AccountTableSettingsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_table_settings_get(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_table_settings_set</a>(...) -> PostV1AccountTableSettingsSetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_table_settings_set(
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

<details><summary><code>client.account.<a href="src/nordlet/account/client.py">post_v1account_table_settings_list</a>() -> PostV1AccountTableSettingsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from nordlet import Nordlet
from nordlet.environment import NordletEnvironment

client = Nordlet(
    token="<token>",
    environment=NordletEnvironment.PRODUCTION,
)

client.account.post_v1account_table_settings_list()

```
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

