# AIml


1) Contenu de `toto.ps1`
Dans `C:\Users\doc\toto.ps1` (à adapter si ton chemin est différent), mets juste :
python "C:\Users\doc\i.py"

ou, si tu veux sans fenêtre console :
pythonw "C:\Users\doc\i.py"
2) Configuration dans le Planificateur de tâches
Dans l’onglet Actions → Nouvelle… :
Programme/script

powershell.exe

Ajouter des arguments (facultatif)

-ExecutionPolicy Bypass -File "C:\Users\doc\toto.ps1"

Oui, tu peux tout à fait utiliser Python directement dans le Planificateur de tâches, sans passer par PowerShell.
1) Sans PowerShell : ce que tu mets
Dans l’onglet Actions → Nouvelle… :
Programme/script
python
(ou le chemin complet, par exemple  
`C:\Users\TonUser\AppData\Local\Programs\Python\Python312\python.exe`  
si Python n’est pas dans le PATH)
si Python n’est pas dans le PATH)
"C:\Users\doc\i.py"
***
https://www.chiny.me/construire-un-reseau-de-neurones-pour-des-donnees-non-lineaires-avec-keras-27-6.php
https://www.scaler.com/topics/keras/keras-simple-model/
https://apxml.com/courses/applied-data-science/chapter-1-advanced-data-acquisition-preparation/web-scraping-techniques
https://github.com/ju4nv1e1r4/agents-with-adk/tree/main
