```mermaid
graph TD
  A[Requisition from Departments] --> B[Submission of Requisition to Storekeeper]
  B --> C[Storekeeper raises Purchase Requisition to Stock Controller]
  C --> D[Stock Controller raises Local Purchase Order]
  D --> E[LPO approved by Directors]
  E --> F[Supplier shares Proforma Invoice]
  F --> G[Receiving Goods]
  G --> H[Security and Stock Controller checks]
  H --> I1[Delivery Note signed]
  H --> I2[Goods Received Note signed]
  H --> I3[Invoice signed]
  I1 --> J[Stock Controller validates quality]
  I2 --> J
  I3 --> J
  J --> K[Stock Controller rejects substandard commodities]
  K --> L[Invoice presented to Director for payment]
  L --> M[Receipt issued upon payment]
  M --> N[Record Keeping with all documents attached]
  N --> O[Issuing Stocks to Departments]
  O --> P[Stock levels updated in inventory system]
  P --> Q[Process Repeats]
