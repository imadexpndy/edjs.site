# EDJS - Plateforme Culturelle

## Description
EDJS est une plateforme culturelle qui connecte les spectacles théâtraux et culturels avec les écoles, associations et familles au Maroc. Notre mission est de rendre la culture accessible à tous.

## Fonctionnalités
- **Pour les Écoles**: Accès gratuit aux spectacles pour les écoles publiques, tarifs préférentiels pour les écoles privées
- **Pour les Associations**: Partenariats et programmes culturels
- **Pour les Familles**: Réservation de billets et découverte de spectacles
- **Pour les Partenaires**: Collaboration et soutien culturel

## Spectacles Disponibles
- Casse-Noisette (Âge 4-12)
- Conte Musical (Âge 3-8)
- Théâtre Jeunesse (Âge 8-15)
- Spectacle Familial (Tout âge)

## Technologies Utilisées
{{ ... }}
- HTML5
- CSS3 (Bootstrap)
- JavaScript (GSAP, Swiper.js, AOS)
- Responsive Design

## 📦 Installation & Setup

### Prerequisites
- Node.js 18+ and npm
- Supabase account and project

### 1. Clone the Repository
```bash
git clone https://github.com/imadexpndy/edjs.site.git
cd edjs.site
```

### 2. Setup Admin App
```bash
cd admin-app
npm install
cp .env.example .env
# Update .env with your Supabase credentials
npm run dev
```

### 3. Setup Website
The website files are now at the root level for easy deployment:
```bash
# Update assets/js/supabase-config.js with your Supabase credentials
# Serve with any static server (Python, Node, etc.)
# The homepage is index.html which will be served automatically
python -m http.server 8000
```

## Structure du Projet
- `index.html` - Page d'accueil
- `about.html` - À propos
- `schools.html` - Page pour les écoles
- `families.html` - Page pour les familles
- `associations.html` - Page pour les associations
- `partners.html` - Page pour les partenaires
- `assets/` - Ressources (CSS, JS, images)

## Contact
- Email: info@edjs.ma
- Téléphone: +212 5 22 98 10 85

## Licence
© 2025 EDJS. Tous droits réservés.
