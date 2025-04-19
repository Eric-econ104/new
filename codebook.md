
### **Codebook for `彰化與全國婚姻情況對比`**

#### **Brief Description**
The `彰化與全國婚姻情況對比` dataset contains normalized marital status data for different regions, age groups, marital statuses, and genders. The dataset calculates the proportion of individuals in each marital status category relative to the total population for a given region and age group. Missing combinations of variables are filled with a proportion of `0`.

---

### **Variable Table**

| **Variable Name** | **Class**   | **Meaning**                                                                                     | **Example**                          |
|--------------------|-------------|-------------------------------------------------------------------------------------------------|--------------------------------------|
| `縣市別`           | Character   | The region or city name. Represents the geographic location of the data.                       | `"彰化縣"`, `"總計"`                 |
| `年齡別`           | Character   | The age group of individuals.                                                                 | `"20-24歲"`, `"25-29歲"`            |
| `婚姻狀況別`       | Character   | The marital status category.                                                                  | `"未婚"`, `"已婚"`, `"離婚"`         |
| `性別`             | Character   | The gender of individuals.                                                                    | `"男"`, `"女"`                       |
| `比例`             | Numeric     | The proportion of individuals in the given marital status category relative to the total.     | `0.25`, `0.5`, `0`                   |

---

### **Dataset Description**
- **Source**: The dataset is derived from '重要性別統計資料庫'https://www.gender.ey.gov.tw/gecdb/Stat_Statistics_Field.aspx
containing marital status data for Changhua County and national totals.
- **Normalization**: The `比例` column is calculated by dividing the count of individuals in a specific marital status by the total count for the corresponding region and age group.
- **Missing Data Handling**: Missing combinations of variables are filled with a proportion of `0` using the `complete()` function.
- **Purpose**: This dataset is useful for analyzing marital status distributions across different regions, age groups, and genders.

---

Let me know if you need further clarification or additional details!
