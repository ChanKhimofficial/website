# Modifier ton site toi-même

## Ce dont tu as besoin

- Un Mac ou PC
- [VS Code](https://code.visualstudio.com/) — éditeur de code gratuit
- [Git](https://git-scm.com/downloads) — pour récupérer et envoyer les fichiers
- Un compte [GitHub](https://github.com) — pour stocker ton site
- Un compte [Vercel](https://vercel.com) — pour mettre en ligne

---

## 1. Récupérer le code sur ton ordi (une seule fois)

Ouvre le **Terminal** (Mac : Cmd+Espace → "Terminal") et tape :

```bash
git clone https://github.com/max-wells/webshipping.git
cd webshipping/sites/chan-khim
code .
```

VS Code s'ouvre avec ton site.

---

## 2. Modifier le site avec une IA

**Option recommandée : [ChatGPT](https://chat.openai.com) ou [Claude](https://claude.ai)**

1. Ouvre `index.html` dans VS Code
2. Copie-colle tout le contenu dans ChatGPT / Claude
3. Dis exactement ce que tu veux changer, ex :  
   *"Change le titre 'Chan Khim' en 'Chan Khim Studio'"*  
   *"Ajoute un lien TikTok dans la section contact"*
4. L'IA te donne le fichier modifié → tu remplaces le contenu de `index.html`

**Option avancée : [Codex / ChatGPT avec accès fichiers]**  
Upload directement `index.html`, demande les modifs, re-télécharge.

---

## 3. Envoyer les changements en ligne

Dans le Terminal (depuis le dossier `chan-khim`) :

```bash
git add .
git commit -m "mise a jour site"
git push origin main
```

Puis redéployer sur Vercel :

```bash
VERCEL_ORG_ID=team_wWXiRW1WA1H6yOEZ0IR6xHTe VERCEL_PROJECT_ID=prj_u1ROz05cD4aV0oZSyeyzmY8sJUo3 vercel --prod --yes
```

Ton site est mis à jour sur **https://chan-khim.vercel.app**

---

## Changer une photo

1. Mets ta nouvelle photo dans `images/gallery01/` (book) ou `images/gallery02/` (polas)
2. Dans `index.html`, remplace le nom du fichier image par le tien
3. Sauvegarde → répète l'étape 3

---

## En cas de problème

Copie l'erreur du terminal et envoie-la à ChatGPT — il t'explique quoi faire.
