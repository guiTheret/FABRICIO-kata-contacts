By inserting contact one by one (INSERT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.041        |
| 100          | 0.327        |
| 10000        | 33.005       |
| 50,000       | 190.784      |
| 100,000      | 408.733      |
| 1,000,000... | ...          |

By inserting by batch of 10000 (SELECT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.000        |
| 100          | 0.001        |
| 10000        | 0.001        |
| 50,000       | 0.002        |
| 100,000      | 0.004        |
| 1,000,000... | 0.06         |

By inserting with index (SELECT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.001        |
| 100          | 0.001        |
| 10000        | 0.001        |
| 50,000       | 0.001        |
| 100,000      | 0.001        |
| 1,000,000... | 0.001        |

Insert with index is slower to insert but is faster to retrieve and constant whatever the numbers of rows.