## Filings
### Endpoints

| Endpoint | Method | Description | Request Body | Params | Response |
|---|---|---|---|---|---|
| `/api/filings/all-filings` | GET | Retrieves a list of [FilingDTO](../api/StockDB.Models.DTO.FilingDTO.yml) objects of company's SEC filings of all types. | None | None | `[{"accessionNum": "0001683168-25-000575", "filingData": "01/29/2025", ...}, ...]` |
| `/api/filings/yearly` | GET | Retrieves a list of [FilingDTO](../api/StockDB.Models.DTO.FilingDTO.yml) objects of company's yearly filings. | None | None | `[{"accessionNum": "0001683168-25-000575", "filingData": "01/29/2025", ...}, ...]` |
| `/api/filings/quarterly` | GET | Retrieves a list of [FilingDTO](../api/StockDB.Models.DTO.FilingDTO.yml) objects of company's quarterly filings. | None | None | `[{"accessionNum": "0001683168-25-000575", "filingData": "01/29/2025", ...}, ...]` |
| `/api/filings/section-sixteen` | GET | Retrieves a list of [FilingDTO](../api/StockDB.Models.DTO.FilingDTO.yml) objects of company's section 16 filings. | None | None | `[{"accessionNum": "0001683168-25-000575", "filingData": "01/29/2025", ...}, ...]` |
| `/api/filings/pdf` | GET | Retrieves pdf document of a filing. | None | String, accession number of filing | pdf file |
| `/api/filings/excel` | GET | Retrieves excel document of a filing. | None | String, accession number of filing | excel file |
| `/api/filings/xbrl-file-documents` | GET | Retrieves xbrl zip file for a filing. | None | String, accession number of filing | xbrl files |


## Usage Examples

### Get all filings

```bash
curl -X GET https://localhost:[port]/api/filings/all-filings
```

### Get all yearly filings 

```bash
curl -X GET https://localhost:[port]/api/filings/yearly
```

### Get all quarterly filings

```bash
curl -X GET https://localhost:[port]/api/filings/quarterly
```

### Get all section 16 filings

```bash
curl -X GET https://localhost:[port]/api/filings/section-sixteen
```

### Get pdf file of a particular filing

```bash
curl -X GET https://localhost:[port]/api/filings/pdf?accessionNum=0001683168-24-001995
```

### Get excel file of a particular filing

```bash
curl -X GET https://localhost:[port]/api/filings/excel?accessionNum=0001683168-24-001995
```

### Get xbrl files of a particular filing

```bash
curl -X GET https://localhost:[port]/api/filings/xbrl-file-documents?accessionNum=0001683168-24-001995
```

