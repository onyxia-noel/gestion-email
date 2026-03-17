# 🤖 Onyxia — Workflows n8n

Automatisations n8n conçues par **Louis Noël** pour gagner du temps et éliminer les tâches répétitives grâce à l'intelligence artificielle.

---

## 📂 Workflows disponibles

### 1. Gmail AI Classifier — Tri automatique des emails par IA

> **Zéro email non trié. Zéro effort manuel.**

Ce workflow analyse chaque email entrant dans Gmail, le fait lire par un agent IA (Groq/GPT), et applique automatiquement le bon label.

**Catégories détectées :**
| Label | Description |
|---|---|
| `IMPORTANT` | Emails prioritaires |
| `FACTURATION` | Factures & paiements |
| `NEW_CLIENT` | Prospects & nouveaux clients |
| `PUB` | Publicités → supprimées automatiquement |
| `PERSONNEL` | Emails personnels |
| `AUTRE` | Tout le reste |

**Stack technique :**
- n8n (automation)
- Gmail API (OAuth2)
- Groq API (LLM)
- JavaScript (code nodes)

**Comment l'installer :**
1. Importer le fichier `workflows/gmail-ai-classifier.json` dans n8n
2. Connecter ton compte Gmail via OAuth2
3. Connecter ton compte Groq (clé API gratuite sur [console.groq.com](https://console.groq.com))
4. Créer les labels Gmail correspondants et remplacer les `Label_XXXX` dans le JSON
5. Activer le workflow ✅

---

## 📸 Aperçu

**Déclencheur Gmail**
![Déclencheur](screenshots/01_declencheur.png)

**Agent IA (Groq)**
![Agent IA](screenshots/02_agent_ia.png)

**Classificateur de mail**
![Classificateur](screenshots/03_classificateur.png)

---

## 👤 À propos

**Louis Noël — Onyxia**
Consultant en automatisation & IA

🔗 [GitHub](https://github.com/onyxia-noel)

---

> Ces workflows sont open-source. Tu peux les réutiliser et les adapter librement.
