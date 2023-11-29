By inserting contact one by one (INSERT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.041        |
| 100          | 0.327        |
| 10000        | 33.005       |
| 50,000       | 190.784      |
| 100,000      | 408.733      |
| 1,000,000... | ...          |

![image](https://github.com/guiTheret/FABRICIO-kata-contacts/assets/95236118/e7a4077c-e931-430d-96e9-d2758122deb2)

By inserting by batch of 10000 (SELECT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.000        |
| 100          | 0.001        |
| 10000        | 0.001        |
| 50,000       | 0.002        |
| 100,000      | 0.004        |
| 1,000,000... | 0.06         |

![image](https://github.com/guiTheret/FABRICIO-kata-contacts/assets/95236118/2219f899-d26c-4151-90af-5ba9e6e3742a)

By inserting with index (SELECT TIME)

| size         | time (in s) |
|--------------|--------------|
| 10           | 0.001        |
| 100          | 0.001        |
| 10000        | 0.001        |
| 50,000       | 0.001        |
| 100,000      | 0.001        |
| 1,000,000... | 0.001        |

![image](https://github.com/guiTheret/FABRICIO-kata-contacts/assets/95236118/e9745b2b-49f3-478a-b039-62d8cf8a71cf)


Insert with index is slower to insert but is faster to retrieve and constant whatever the numbers of rows.
