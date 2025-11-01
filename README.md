 # TP 13 : Sérialisation

 ##  Exercice 1  : Sérialisation simple avec `Serializable`

##  Objectif
Apprendre à sauvegarder et restaurer des objets en Java à l’aide de l’interface `Serializable`.  
Cet exercice montre comment écrire et relire des objets dans un fichier binaire à l’aide des flux d’objets (`ObjectOutputStream` et `ObjectInputStream`).

---
 ##  Sortie attendue
 ```
→ Sérialisation réussie dans employees.ser
→ Désérialisation réussie, objets restaurés :
  Employee[id=1, name=Youssef, salary=3000.00, password=null]
  Employee[id=2, name=Fatima,  salary=3500.50, password=null]
  Employee[id=3, name=Omar,    salary=2800.75, password=null]

Note : le champ 'password' est transient, il n’a pas été enregistré → null.

```
##  Exemple d’exécution (image)
 
Voici un exemple de l'exécution du programme (screenshot) :


 ## Exercice 2 : Sérialisation Avancée avec Externalizable et Contrôle de Flux

##  Objectifs pédagogiques
- Découvrir l’interface **`Externalizable`** pour un contrôle total de la sérialisation.  
- Implémenter manuellement les méthodes `writeExternal()` et `readExternal()`.  
- Manipuler des champs **transients** et des **données dérivées**.  
- Comprendre la différence entre `Serializable` et `Externalizable`.  
- Versionner manuellement le format binaire pour assurer la compatibilité.

---

 ## Sortie console attendue
 ```
Historique sauvegardé dans chat.ser
Historique chargé :
  [18 chars] 2025-11-01T21:35:12.154Z [Youssef]: Salam tout le monde
  [20 chars] 2025-11-01T21:35:12.155Z [Fatima]: Wa ʿalaykum as-salām
  [17 chars] 2025-11-01T21:35:12.156Z [Omar]: Comment ça va ?

```
##  Exemple d’exécution (image)
 
Voici un exemple de l'exécution du programme (screenshot) :


