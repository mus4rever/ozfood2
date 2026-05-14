# Ozfood Website

Site vitrine premium pour Ozfood, grossiste snack & horeca en Belgique.

## Stack

- Next.js 14 App Router
- TypeScript
- Tailwind CSS
- Composants réutilisables
- Structure multilingue prête pour `fr`, `nl`, `en`

## Lancer le projet

```bash
npm install
npm run dev
```

Le site démarre sur `http://localhost:3000`.

## Variables à configurer

Copier `.env.example` vers `.env.local`, puis remplacer :

```bash
NEXT_PUBLIC_SITE_URL=https://www.ozfood.be
NEXT_PUBLIC_WEBSHOP_URL=https://votre-lien-monadem
NEXT_PUBLIC_WHATSAPP_URL=https://wa.me/32475330110
NEXT_PUBLIC_PHONE=02 201 31 55
NEXT_PUBLIC_APPSTORE_URL=
NEXT_PUBLIC_PLAYSTORE_URL=
NEXT_PUBLIC_ADDRESS=Schaerbeeklei 724, 1800 Vilvoorde
```

Les liens externes sont utilisés dans `lib/links.ts`, puis consommés partout via `data/site.ts`.

## Contacts configurés

Les contacts se trouvent dans `lib/links.ts` :

- Téléphone : `02 201 31 55`
- WhatsApp commande : `0475 33 01 10`
- Adresse : `Schaerbeeklei 724, 1800 Vilvoorde`

## Images et logo

Les logos officiels optimisés sont dans `public/images/brand` :

- `ozfood-logo-color.png`
- `ozfood-logo-white.png`
- `ozfood-logo-black.png`

Les images temporaires produits/logistique sont déclarées dans `data/media.ts`.

À remplacer idéalement par des assets Ozfood réels :

- Hero burger / snack
- Burgers & pains
- Snacks & viandes halal
- Frites & accompagnements
- Sauces & condiments
- Boissons
- Emballages
- Camion Ozfood
- Entrepôt Ozfood
- Photo contact / équipe

## Pages

- `/fr`
- `/fr/qui-sommes-nous`
- `/fr/notre-selection`
- `/fr/promotions`
- `/fr/application`
- `/fr/clients`
- `/fr/logistique`
- `/fr/contact`

Les routes `/nl` et `/en` sont déjà prévues dans la structure.

## Mémoire stratégique intégrée

- Le site reste une vitrine commerciale, pas un faux webshop.
- Le site vend l’envie, Monadem gère la commande.
- L’application mobile Ozfood est prévue comme deuxième chemin de commande.
- WhatsApp est gardé comme outil humain d’aide et de conversion.
- Les catégories principales couvrent burgers, pains, snacks halal, frites, sauces, boissons, boulangerie, produits laitiers et emballages.
- Le formulaire de contact prépare un message WhatsApp, faute d’endpoint email/CRM fourni.
- Le bandeau haut et le pop-up sont configurables dans `data/announcements.ts`.
