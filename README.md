# Bankruptcy-Prediction

API RESTful to use Bankrupcty predictor model

## How to Use

Pull the repository and write the following command in your cmd

```
uvicorn api.main:app
```

Then, you can consume the API from localhost:8000

Executing with Docker is easier than previous one, Just run docker compose file with the following command in the cmd

```
docker-compose up -d
```

Then, you can consume the API from localhost:8000

## JSON Structure
You have to pass the following JSON structure to get a request

```
{
    "val_1": "float number",
    "val_2": "float number",
    "val_3": "float number",
    "val_4": "float number",
    "val_5": "float number",
    "val_6": "float number",
    "val_7": "float number",
    "val_8": "float number",
    "val_9": "float number",
    "val_10": "float number",
    "val_11": "float number",
    "val_12": "float number",
    "val_13": "float number",
    "val_14": "float number",
    "val_15": "float number",
    "val_16": "float number",
    "val_17": "float number",
    "val_18": "float number",
    "val_19": "float number",
    "val_20": "float number"
}
```

Where these val_x values are respectively:
- ROA(C) before interest and depreciation before interest
- ROA(A) before interest and % after tax
- ROA(B) before interest and depreciation after tax
- Tax rate (A)
- Net Value Per Share (B)
- Net Value Per Share (A)
- Net Value Per Share (C)
- Persistent EPS in the Last Four Seasons
- Operating Profit Per Share (Yuan ¥)
- Per Share Net profit before tax (Yuan ¥)
- Debt ratio %
- Net worth/Assets
- Operating profit/Paid-in capital
- Net profit before tax/Paid-in capital
- Working Capital to Total Assets
- Cash/Total Assets
- Current Liability to Assets
- Retained Earnings to Total Assets
- Current Liability to Current Assets
- Net Income to Total Assets

That's all, now consume the API and have fun :smile:
