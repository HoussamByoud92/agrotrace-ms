# Architecture Overview

## System Architecture

```mermaid
graph TB
    A[Capteurs IoT] --> B[IngestionCapteurs]
    C[Stations Météo] --> B
    D[Images UAV] --> E[Prétraitement]
    
    B --> F[Kafka]
    E --> F
    
    F --> G[VisionPlante]
    F --> H[PrévisionEau]
    
    G --> I[RèglesAgro]
    H --> I
    
    I --> J[RecoIrrigation]
    J --> K[DashboardSIG]
    
    K --> L[Utilisateur Agriculteur]