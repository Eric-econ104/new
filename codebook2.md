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

以下是基於您提供的正確資料建立的 Markdown 檔案：

---

# **Summary of `彰化與全台婚姻對比`**

## **1. Summary of Numerical Statistics**

| **Variable** | **Statistic** | **Value**                                   |
|--------------|---------------|---------------------------------------------|
| 比例         | Mean          | 0.166666666666667                           |
| 比例         | Median        | 0.0739707442714029                          |
| 比例         | SD            | 0.179428783614078                           |
| 比例         | Max           | 0.701600829206495                           |
| 比例         | Min           | 6.79965745493749e-05                        |
| 比例         | Range         | 6.79965745493749e-05, 0.701600829206495     |
| 113年        | Mean          | 93550.0601851852                            |
| 113年        | Median        | 11131.5                                     |
| 113年        | SD            | 173975.029078931                            |
| 113年        | Max           | 683329                                      |
| 113年        | Min           | 1                                           |
| 113年        | Range         | 1, 683329                                   |

---

## **2. Summary of Missing Data**

| **Variable**   | **Total Missing** | **Percentage Missing** |
|----------------|-------------------|-------------------------|
| 縣市別         | 0                 | 0%                      |
| 年齡別         | 0                 | 0%                      |
| 婚姻狀況別     | 0                 | 0%                      |
| 性別           | 0                 | 0%                      |
| 比例           | 0                 | 0%                      |
| 113年          | 0                 | 0%                      |

---

## **3. Summary of Factors**

### **3.1 縣市別**
- **Class**: Factor
- **Frequency Table**:
  ```
  彰化縣    108
  總計      108
  ```

### **3.2 年齡別**
- **Class**: Factor
- **Frequency Table**:
  ```
  100歲以上    12
  15-19歲     12
  20-24歲     12
  25-29歲     12
  30-34歲     12
  35-39歲     12
  40-44歲     12
  45-49歲     12
  50-54歲     12
  55-59歲     12
  60-64歲     12
  65-69歲     12
  70-74歲     12
  75-79歲     12
  80-84歲     12
  85-89歲     12
  90-94歲     12
  95-99歲     12
  ```

### **3.3 婚姻狀況別**
- **Class**: Factor
- **Frequency Table**:
  ```
  未婚    72
  有偶    72
  離婚    72
  ```

### **3.4 性別**
- **Class**: Factor
- **Frequency Table**:
  ```
  女    108
  男    108
  ```

---

### **Notes**
1. **Numerical Statistics**:
   - The `比例` column represents proportions, with a range of `6.79965745493749e-05` to `0.701600829206495`.
   - The `113年` column represents population counts, with a range of `1` to `683329`.

2. **Missing Data**:
   - No missing data was found in any variable.

3. **Factors**:
   - Frequency tables for categorical variables (`縣市別`, `年齡別`, `婚姻狀況別`, `性別`) are included.

---




