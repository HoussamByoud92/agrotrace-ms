# AgroTrace-MS

Platforme intelligente de surveillance des cultures et d'optimisation de l'irrigation.

## Architecture Microservices

- **IngestionCapteurs**: Collecte données IoT
- **Prétraitement**: Nettoyage et segmentation
- **VisionPlante**: Détection maladies IA
- **PrévisionEau**: Prédiction besoins irrigation
- **RèglesAgro**: Moteur de règles métier
- **RecoIrrigation**: Génération recommandations
- **DashboardSIG**: Interface visualisation

## Démarrage Rapide

```bash
git clone https://github.com/AgroTrace-MS/agrotrace-ms.git
cd agrotrace-ms
docker-compose up -d
