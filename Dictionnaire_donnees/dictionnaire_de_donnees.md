# APP_USER :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant Unique/ Object_id | ID de l'utilisteur |
| firstname | STRING | Not Null | Prénom de l'utilisateur |
| lastname | STRING | Not Null | Nom de l'utilisateur |
| email | STRING | Not Null, Unique | Email de l'utilisateur |
| hashed_password | STRING | Not Null, Hashed  | Mot de passe de l'utilisateur |
| status | STRING | ADMIN, USER, AUTHOR | Rôle de l'utilisateur |
| created_at | DATE | Not Null, Date.now() | Date de création de l'utilisateur |
| updated_at | DATE | Null, Date.now() | Date de modification de l'utilisateur |


# QUIZ :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant unique/Object_id | ID du quiz |
| title | STRING | Not Null | Titre du quiz |
| quiz_description | STRING | Not Null | Description du quiz |
| status | STRING | Not Null | Status du quiz |
| created_at | DATE | Not Null, Date.now() | Date de création du quiz |
| updated_at | DATE | Not Null, Date.now() | Date de modification du quiz |


# TAG :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant unique/Object_id | ID du tag |
| tag_name | STRING | Not Null | Nom du tag |
| status | STRING | Not Null | Status du tag |
| created_at | DATE | Not Null, Date.now() | Date de création du tag |
| updated_at | DATE | Null, Date.now() | Date de modification du tag |


# QUESTION :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant unique/Object_id | ID de la question |
| question_content | STRING | Not Null | Intitulé de la question |
| anecdote | STRING | Null | Anecdote(s) reliée(s) à la question |
| wiki | STRING | Null | Lien wikipédia relié à la question |
| status | STRING | Not Null | Status de la question |
| created_at | DATE | Not Null, Date.now() | Date de création de la question |
| updated_at | DATE | Null, Date.now() | Date de modification de la question |


# ANSWER :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant unique/Object_id | ID de la réponse |
| answer_description | STRING | Not Null | Intitulé de la réponse |
| status | STRING | Not Null | Status de la réponse |
| created_at | DATE | Not Null, Date.now() | Date de création de la réponse |
| updated_at | DATE | Null, Date.now() | Date de modification de la réponse |


# LEVEL :
|Champ|Type|Spécificités|Description|
|-|-|-|-|
| id | STRING | Identifiant unique/Object_id | ID du niveau |
| level_name | STRING | Not Null, EASY/MEDIUM/HARD | Intitulé du niveau |
| status | STRING | Not Null | Status du niveau |
| created_at | DATE | Not Null, Date.now() | Date de création du niveau |
| updated_at | DATE | Null, Date.now() | Date de modification du niveau |