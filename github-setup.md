# 🚀 Guide de Déploiement GitHub + Netlify

## Étape 1 : Créer le Repository GitHub

### 1.1 Créer le Repository
1. Aller sur [github.com](https://github.com)
2. Cliquer "New repository" (bouton vert)
3. **Nom du repository :** `nadia-hajjoub-portfolio`
4. **Description :** `Portfolio professionnel de Nadia Hajjoub - Sociologue & Chercheuse`
5. ✅ Cocher "Public" (pour Netlify gratuit)
6. ✅ Cocher "Add a README file"
7. Cliquer "Create repository"

### 1.2 Uploader les Fichiers
**Option A : Via l'interface GitHub (Plus Simple)**
1. Dans le repository, cliquer "uploading an existing file"
2. Glisser tous les fichiers du portfolio (sauf README.md)
3. **Commit message :** `Initial portfolio upload`
4. Cliquer "Commit changes"

**Option B : Via Git (Plus Pro)**
```bash
# Dans le terminal, aller dans le dossier du portfolio
cd "/Users/viet/Desktop/Nadia website"

# Initialiser Git
git init

# Ajouter l'origine GitHub (remplacer USERNAME)
git remote add origin https://github.com/USERNAME/nadia-hajjoub-portfolio.git

# Ajouter tous les fichiers
git add .

# Premier commit
git commit -m "Initial portfolio upload - Nadia Hajjoub"

# Pousser vers GitHub
git push -u origin main
```

## Étape 2 : Connecter Netlify

### 2.1 Créer Compte Netlify
1. Aller sur [netlify.com](https://netlify.com)
2. Cliquer "Sign up" 
3. **Choisir "GitHub"** pour se connecter
4. Autoriser Netlify à accéder à GitHub

### 2.2 Déployer le Site
1. Dans Netlify, cliquer "Add new site"
2. Choisir "Import an existing project"
3. Sélectionner "GitHub"
4. Chercher et sélectionner `nadia-hajjoub-portfolio`
5. **Build settings :**
   - Build command : `(laisser vide)`
   - Publish directory : `(laisser vide ou mettre ".")`
6. Cliquer "Deploy site"

### 2.3 Configuration du Site
1. **Changer le nom du site :**
   - Aller dans "Site settings" > "General"
   - Cliquer "Change site name"
   - Nouveau nom : `nadia-hajjoub-portfolio`
   - URL finale : `nadia-hajjoub-portfolio.netlify.app`

2. **Domaine personnalisé (Optionnel) :**
   - Aller dans "Domain settings"
   - Cliquer "Add custom domain"
   - Entrer : `nadiahajjoub.com` (si acheté)

## Étape 3 : Vérifications

### 3.1 Tests Essentiels
- ✅ Site accessible via l'URL Netlify
- ✅ Navigation fonctionne sur mobile
- ✅ Images se chargent correctement
- ✅ Formulaire de contact opérationnel
- ✅ Responsive sur tous appareils

### 3.2 Optimisations Post-Déploiement
- 📊 Ajouter Google Analytics (optionnel)
- 🔍 Vérifier le SEO avec Lighthouse
- ⚡ Tester la vitesse sur PageSpeed Insights
- 📱 Tester sur différents navigateurs

## 🎯 Résultat Final

**URL du Portfolio :** `https://nadia-hajjoub-portfolio.netlify.app`

**Avantages de cette méthode :**
- ✅ Déploiement automatique à chaque mise à jour GitHub
- ✅ Historique des versions avec Git
- ✅ Collaboration possible avec d'autres développeurs
- ✅ Sauvegarde automatique sur GitHub
- ✅ URL professionnelle et mémorable
- ✅ HTTPS automatique et sécurisé

## 🔄 Mises à Jour Futures

Pour modifier le site :
1. Modifier les fichiers localement
2. `git add .`
3. `git commit -m "Description des changements"`
4. `git push`
5. ✅ Netlify redéploie automatiquement !

## 📞 Support

- **Documentation Netlify :** [docs.netlify.com](https://docs.netlify.com)
- **GitHub Help :** [docs.github.com](https://docs.github.com)
- **Communauté :** Stack Overflow, Reddit
