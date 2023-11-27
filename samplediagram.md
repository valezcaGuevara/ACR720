```mermaid
graph TD
  subgraph PayPalAPI[PAYPAL API]
    subgraph Users[Users]
      User1
      User2
    end
    subgraph ExternalSystem[External System]
      ExternalApp
    end
  end

  User1 -->|Uses| PayPalAPI
  User2 -->|Uses| PayPalAPI
  ExternalApp -->|Sends payment request to| PayPalAPI
```
