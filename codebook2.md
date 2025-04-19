Here is a Markdown codebook for the `彰化與全台婚姻情況對比` dataset:

---

# **Codebook for `彰化與全台婚姻情況對比`**

## **Dataset Description**
The `finally_parsed` dataset contains normalized marital status data for different regions, age groups, marital statuses, and genders. It includes the total population (`113年`) and the proportion (`比例`) of individuals in each marital status category relative to the total population for a given region and age group.

---

## **Variable Table**

| **Variable Name** | **Class**   | **Description**                                                                                 | **Example**                          |
|--------------------|-------------|-------------------------------------------------------------------------------------------------|--------------------------------------|
| `縣市別`           | Factor      | The region or city name. Represents the geographic location of the data.                       | `"彰化縣"`, `"總計"`                 |
| `年齡別`           | Factor      | The age group of individuals.                                                                 | `"20-24歲"`, `"25-29歲"`            |
| `婚姻狀況別`       | Factor      | The marital status category.                                                                  | `"未婚"`, `"已婚"`, `"離婚"`         |
| `性別`             | Factor      | The gender of individuals.                                                                    | `"男"`, `"女"`                       |
| `比例`             | Numeric     | The proportion of individuals in the given marital status category relative to the total.     | `0.25`, `0.5`, `0`                   |
| `113年`            | Numeric     | The total population count for the given combination of variables.                           | `1000`, `500`, `0`                   |

---

## **Dataset Details**
- **Source**: Derived from marital status data for Changhua County and national totals.`重要性別統計資料庫`https://www.gender.ey.gov.tw/gecdb/Stat_Statistics_Field.aspx 
- **Normalization**: The `比例` column is calculated by dividing the count of individuals in a specific marital status by the total count for the corresponding region and age group.
- **Missing Data Handling**: Missing combinations of variables are filled with a proportion of `0` and a population count of `0` using the `complete()` function.
- **Purpose**: This dataset is useful for analyzing marital status distributions across different regions, age groups, and genders between 彰化和全台婚姻情況。

---

## **Example Rows**

| 縣市別   | 年齡別     | 婚姻狀況別 | 性別 | 比例  | 113年 |
|----------|------------|------------|------|-------|-------|
| 彰化縣   | 20-24歲    | 未婚       | 男   | 0.45  | 450   |
| 彰化縣   | 20-24歲    | 已婚       | 女   | 0.10  | 100   |
| 總計     | 25-29歲    | 離婚       | 男   | 0.05  | 50    |
| 總計     | 25-29歲    | 未婚       | 女   | 0.40  | 400   |

---


