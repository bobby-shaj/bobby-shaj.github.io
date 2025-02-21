## Stocks
### Endpoints

| Endpoint | Method | Description | Request Body | Params | Response |
|---|---|---|---|---|---|
| `/api/stock` | GET | Retrieves a list of [StockDTO](../api/StockWebAPI.Models.StockDTO.yml/) objects. | None | Stock index | `[{"isAfterHrs": true, "today": {"last": "1.476", ...}, ...}, ...]` |
| `/api/stock/stockoneday` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for today. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stockfivedays` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past five days. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stockonemonth` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past month. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stockthreemonths` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past three months. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stocksixmonths` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past six months. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stockoneyear` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past year. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stocktwoyears` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past two years. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/stockfiveyears` | GET | Retrieves a list of [StockDataPointDTO](../api/StockWebAPI.Models.StockDataPointDTO.yml/) objects for past five years. | None | Stock index | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |
| `/api/stock/historicaldata` | GET | Retrieves a list of [DailyDataDTO](../api/StockWebAPI.Models.DailyDataDTO.yml/) objects for the specified period of time. | None | Stock index, start date, end date | `[{"Title": "Thursday...", "index": "fcuv", ...}, ...]` |


## Usage Examples

### Get stock data

```bash
curl -X GET https://localhost:[port]/api/stock?index=[stock symbol]
```

### Get today's stock datapoints

```bash
curl -X GET https://localhost:[port]/api/stock/stockoneday?index=[stock symbol]
```

### Get last five days' stock datapoints

```bash
curl -X GET https://localhost:[port]/api/stock/stockfivedays?index=[stock symbol]
```

### Get stock datapoints for the past month

```bash
curl -X GET https://localhost:[port]/api/stock/stockonemonth?index=[stock symbol]
```

### Get stock datapoints for the past three months

```bash
curl -X GET https://localhost:[port]/api/stock/stockthreemonths?index=[stock symbol]
```

### Get stock datapoints for the past six months

```bash
curl -X GET https://localhost:[port]/api/stock/stocksixmonths?index=[stock symbol]
```

### Get stock datapoints for previous year

```bash
curl -X GET https://localhost:[port]/api/stock/stockoneyear?index=[stock symbol]
```

### Get stock datapoints for previous two years

```bash
curl -X GET https://localhost:[port]/api/stock/stocktwoyears?index=[stock symbol]
```

### Get stock datapoints for past five years

```bash
curl -X GET https://localhost:[port]/api/stock/stockfiveyears?index=[stock symbol]
```

### Get historical data points for a given stock symbol

```bash
curl -X GET https://localhost:[port]/api/stock/historicaldata?index=[stock symbol]&start=[start-date]&end=[end-date]
```