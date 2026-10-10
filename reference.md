# Reference
## reference
<details><summary><code>client.reference.<a href="src/nordlet/reference/client.py">exchange_rates_sync</a>(...) -> ExchangeRatesSyncReferenceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.partners.<a href="src/nordlet/partners/client.py">validate_vat</a>(...) -> ValidateVatPartnersResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

Send an issued invoice or credit note to the customer over Peppol through the company's own access point (Settings → Compliance → EU; Nordlet supports Recommand, Storecove and e-invoice.be). Without one the call is refused with 422 and the document can only be downloaded with `sales/invoices/peppol-xml`. `status` is `pending` until the receiving access point confirms, then `delivered`; `failed` and `rejected` come with `detail`, and the invoice can then be sent again. Later changes arrive through the access point's webhook and are announced as `sale_invoice.peppol_delivered`, `sale_invoice.peppol_rejected` and `sale_invoice.peppol_failed`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.sales.<a href="src/nordlet/sales/client.py">recognition_compute</a>(...) -> RecognitionComputeSalesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

Build the working paper for the Form B1 annual return of a financial year - company details, registered office, directors and secretary from Settings → Officers, the members from Settings → Shareholders, the issued share capital and the figures of the financial statements - in the order the CORE screens ask for them. The CRO publishes no file format for the B1, so it is keyed into CORE.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.declarations.<a href="src/nordlet/declarations/client.py">configs_list</a>() -> ConfigsListDeclarationsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

**translations:** `typing.Optional[typing.Dict[str, AccountsCreateLedgerRequestTranslationsValue]]` 
    
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

#### 🔌 Usage

<dl>
<dd>

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

**translations:** `typing.Optional[typing.Dict[str, typing.Optional[AccountsUpdateLedgerRequestTranslationsValue]]]` 
    
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

#### 🔌 Usage

<dl>
<dd>

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

Replaces the seeded chart with the chart template of the company country (the Romanian general chart for a company registered in Romania, the Lithuanian standard chart otherwise) and switches the posting defaults with it. Answers 409 when the company already uses that chart, has journal entries, holds accounts created by hand, or has settings that name an account the new chart does not have.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

The rows or codes of each return or registry deposit of the company country that are filled from account balances. Accounts fall into a row by the layout defaults for the standard chart of accounts unless mapped under Settings → Statement rows.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.payroll.<a href="src/nordlet/payroll/client.py">calc</a>(...) -> CalcPayrollResponse</code></summary>
<dl>
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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">import_templates_list</a>(...) -> ImportTemplatesListBankResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.bank.<a href="src/nordlet/bank/client.py">feeds_banks_list</a>(...) -> FeedsBanksListBankResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

<details><summary><code>client.billing.<a href="src/nordlet/billing/client.py">topup_create</a>(...) -> TopupCreateBillingResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

#### 🔌 Usage

<dl>
<dd>

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

