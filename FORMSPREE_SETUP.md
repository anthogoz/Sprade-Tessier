# Configuration FormSpree pour le formulaire de contact

## Étapes pour activer le formulaire de contact

### 1. Créer un compte FormSpree
1. Visitez https://formspree.io
2. Créez un compte gratuit (ou connectez-vous si vous en avez déjà un)
3. Le plan gratuit permet 50 soumissions par mois

### 2. Créer un nouveau formulaire
1. Une fois connecté, cliquez sur "+ New Form"
2. Nommez votre formulaire : "Contact Sprade"
3. FormSpree vous donnera un ID de formulaire unique (format : `xpzgqwer` par exemple)

### 3. Configurer l'email de réception
1. Dans les paramètres du formulaire, configurez l'email de destination : `pierre.tessier88100@gmail.com`
2. Vous pouvez personnaliser le message de confirmation envoyé aux utilisateurs

### 4. Mettre à jour le fichier index.html
Dans le fichier `index.html`, ligne 250, remplacez :
```html
<form class="contact-form glass-card" id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Par :
```html
<form class="contact-form glass-card" id="contactForm" action="https://formspree.io/f/VOTRE_ID_ICI" method="POST">
```

**Remplacez `VOTRE_ID_ICI` par l'ID unique fourni par FormSpree.**

### 5. Tester le formulaire
1. Ouvrez votre site web
2. Remplissez le formulaire de contact
3. Cliquez sur "Envoyer le message"
4. Vous devriez recevoir un email de notification
5. La première soumission nécessitera une confirmation de l'adresse email

## Fonctionnalités incluses

✅ Validation côté client (email, téléphone, champs requis)
✅ Protection anti-spam intégrée par FormSpree
✅ Messages d'état (succès/erreur) avec notifications visuelles
✅ Indicateur de chargement pendant l'envoi
✅ Réinitialisation automatique du formulaire après envoi

## Options avancées (plan payant)

Si vous souhaitez plus de fonctionnalités :
- Soumissions illimitées
- Fichiers joints
- Intégrations (Slack, Google Sheets, etc.)
- Webhooks personnalisés
- Suppression du branding FormSpree

## Alternative gratuite

Si vous préférez une solution entièrement gratuite et sans limite :
- **Netlify Forms** : Si votre site est hébergé sur Netlify
- **Google Forms** : Intégration possible mais moins élégante
- **Backend personnalisé** : Nécessite un serveur

## Support

En cas de problème :
- Documentation FormSpree : https://help.formspree.io
- Email support : support@formspree.io

