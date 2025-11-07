# Admin-Poste-Exercice-3-Intermediaire

Pour cet exercice, j’ai extrait les logs du service SSH sur les dernières 24 heures, filtré uniquement les connexions échouées, et sauvegardé le résultat dans un fichier texte. J’ai travaillé depuis PowerShell en SSH sur ma machine Linux.

# 1) Afficher les logs SSH (24h)

<img width="1919" height="143" alt="image" src="https://github.com/user-attachments/assets/39d2aa28-5886-42d3-948c-152f51b4bca8" />

# 2) Filtrer uniquement les connexions ratées

<img width="1919" height="97" alt="image" src="https://github.com/user-attachments/assets/c6add1eb-1be3-4df1-bfdc-ce4af89c8d61" />

J’ai volontairement généré un échec de connexion SSH pour tester le filtrage. On voit bien la ligne Failed password.

# 3) Sauvegarder les logs filtrés dans un fichier

<img width="1919" height="69" alt="image" src="https://github.com/user-attachments/assets/104e01f7-0b7a-43df-985e-aae3ef38ed6d" />

Vérification du fichier :

<img width="1919" height="135" alt="image" src="https://github.com/user-attachments/assets/c42e376b-1e4f-4708-b10a-88df4e91dcae" />

<img width="1919" height="70" alt="image" src="https://github.com/user-attachments/assets/c3fc5417-d290-495f-843a-e4e329a4b295" />

Dans mon cas, c’est l’adresse 192.168.56.1 qui a généré la tentative échouée.

# Conclusion

J’ai appris à analyser les logs SSH avec journalctl, extraire les tentatives de connexion ratées, puis les sauvegarder dans un fichier pour consultation future. Cette méthode permet de surveiller facilement les essais d’intrusion ou d’échecs répétés sur le système.
