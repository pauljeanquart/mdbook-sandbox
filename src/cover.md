<p align="center">
  <img alt="Software Skills Iceberg" width="425" height="550" src="images/iceberg.png">
<br />
HL Modern Development
</p>

![image](https://github.com/pauljeanquart/mdbook-sandbox/assets/728239/056a7092-13e6-400c-9078-acff186e0c4c)

```mermaid
erDiagram
    VENDOR ||--o{ INVOICE : "requests payments"
    VENDOR {
        int VendorID PK
        string VendorName
    }
    INVOICE ||--|{ DETAIL : contains
    INVOICE {
        int InvoiceID PK
        string VendorID FK
        string InvoiceNumber
    }
    DETAIL {
        int InvoiceID PK,FK "Part of compound primary key"
        int InvoiceSequence PK "Part of compound primary key"
        string ItemDescription
    }
```


```sql
SELECT *
FROM Company
WHERE
  CompanyID = 2;
```
