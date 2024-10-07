<<<<<<< HEAD
# MermaidAsma.github.io

```mermaid
erDiagram
    CUSTOMER {
        int customer_id PK "Primary Key"
        string name
        string email
        string phone_number
    }

    PRODUCT {
        int product_id PK "Primary Key"
        string NIKE model_name
        string size
        string price
    }

    SALES {
        int sale_id PK "Primary Key"
        int customer_id FK "Foreign Key"
        int product_id FK "Foreign Key"
        date sale_date
        int quantity
    }

    INVENTORY {
        int inventory_id PK "Primary Key"
        int product_id FK "Foreign Key"
        int stock_level
    }

    CUSTOMER ||--o{ SALES : "makes"
    PRODUCT ||--o{ SALES : "is sold in"
    PRODUCT ||--|| INVENTORY : "has"

# *_Description of the diagram_*:

The ERD diagram is efficient to manage the inventory, sales transaction, and costumers information.
The relationships created are:
- Relationship between COSTUMER and SALES.
- Relationship between PRODUCT and SALES: One model of shoes can be part of many sales
- Relationship between PRODUCT and INVENTORY: A PRODUCT has one inventory or stock record.




