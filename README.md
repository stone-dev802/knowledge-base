
# Mini Knowledge Base – Base de connaissances collaborative 📚


## Présentation du projet 📝
Ce projet est une base de connaissances collaborative réalisée dans le cadre d'un TPE académique.  
Il regroupe des fiches pédagogiques rédigées en Markdown sur les thèmes suivants :  
- Git & GitHub  
- Méthodes Agiles  
- Bonnes pratiques de développement  

**Objectif pédagogique :** travailler dans des conditions proches du monde professionnel en utilisant Git, GitHub et une organisation Agile.

**🎯 Objectifs pédagogiques détaillés :**
- Utiliser Git de manière professionnelle en local  
- Travailler en équipe avec GitHub  
- Appliquer un workflow Git utilisé en entreprise  
- Organiser le travail avec une approche Agile  
- Mettre en place une intégration continue simple  

## Structure du dépôt 📁
knowledge-base/
│── README.md
│── CONTRIBUTING.md
│── docs/
│ ├── git/
│ │ ├── git-init.md
│ │ ├── branches.md
│ ├── agile/
│ │ ├── scrum.md
│ │ ├── kanban.md
│── actifs/ 

- `/docs` : fiches pédagogiques  
- `/actifs` : images ou fichiers supports  
- `README.md` : documentation principale  
- `CONTRIBUTING.md` : règles de contribution 

## Organisation Agile 🧩
- **Méthode :** Kanban  
- **Outils :**  
  - Issues GitHub pour le backlog  
  - Projets GitHub pour le tableau Kanban  
- **Colonnes du Kanban :** Backlog → In Progress → Review → Done  

**User Stories :**  
Chaque Issue correspond à une User Story :  

**Exemples :**
- En tant qu’étudiant, je veux ajouter une fiche pédagogique afin de compléter la base de connaissances  
- En tant que membre du groupe, je veux relire les fiches ajoutées afin de garantir leur qualité  
- En tant qu’utilisateur, je veux naviguer facilement dans le dépôt afin de retrouver les informations rapidement  


## Workflow Git utilisé 🔀
**Workflow : GitHub Flow**  
- Branche principale protégée (`main`)  
- Une branche par fonctionnalité : `feature/<nom-fonctionnalité>`  
- Pull Request obligatoire pour fusionner  
- Revue par au moins un membre avant fusion  

**Exemple de workflow :**
```bash
git checkout -b feature/ajout-fiche
git add .
git commit -m "Ajout d'une nouvelle fiche sur Git"
git push -u origin feature/ajout-fiche
gh pr create --base main --head feature/ajout-fiche --title "Ajout fiche Git" --body "Description"
gh pr merge feature/ajout-fiche --merge 
