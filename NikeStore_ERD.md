<<<<<<< HEAD
# MermaidAsma.github.io

```mermaid
erDiagram
 PRODUCT ||--o{ SALES : "is sold in"
 PRODUCT ||--o{ INVENTORY : "is tracked in"
 PRODUCT {
        int shoes_id PK "Primary Key"
        string NIKE_model name
        string size
 }
 CUSTOMER ||--o{ SALES : "makes"
  CUSTOMER {
        int customer_id PK "Primary Key"
        string name
        string email
        string phone_number
 
 }
 SALE {
        int sale_id PK "Primary Key"
        int customer_id FK "Foreign Key"
        int shoes_id FK "Foreign Key"
        date sale_date
 }
 INVENTORY {
        int inventory_id PK "Primary Key"
        int shoes_id FK "Foreign Key"
        int quantity in stock
 }
 
```
=======


