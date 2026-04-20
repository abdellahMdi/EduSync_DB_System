<img width="632" height="337" alt="image" src="https://github.com/user-attachments/assets/a997b05e-4240-40b4-b227-e601764850ed" />


## Cardinalités des Relations

### Tableau récapitulatif

| Table A | Relation | Table B | Cardinalité | Explication |
|---------|----------|---------|-------------|-------------|
| `roles` | contient → | `users` | **1:N** | Un rôle peut être attribué à plusieurs utilisateurs. Un utilisateur n'a qu'un seul rôle. |
| `users` | possède → | `students` | **1:1** | Un utilisateur peut être un étudiant (profil unique). Un profil étudiant est lié à exactement un compte utilisateur. |
| `users` | enseigne → | `courses` | **1:N** | Un professeur (utilisateur avec rôle "Prof") peut enseigner plusieurs cours. Un cours n'est assigné qu'à un seul professeur. |
| `classes` | regroupe → | `students` | **1:N** | Une classe contient plusieurs étudiants. Un étudiant appartient à une seule classe. |
| `students` | s'inscrit → | `courses` | **N:N** | Un étudiant peut s'inscrire à plusieurs cours. Un cours peut accueillir plusieurs étudiants. |
| `enrollments` | fait le lien entre → | `students` & `courses` | Table de jointure | Résout la relation N:N entre `students` et `courses`. |

---
