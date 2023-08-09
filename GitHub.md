## <font color = "chartreuse">Comment utiliser GitHub ?</font> 👍

![[github-logo-vector 1.png]]
![[CheatSheet_GitHub.png]]

### <font color = "yellow">Versionner en local</font>
---

```github
git init

# Aller dans le dossier de travail > initialiser le dépôt
```

```github
git add .

# Ajoute toutes les modifications (le . symbolise tout)
	C'est à dire qu'on prend tous les fichiers de notre dossier et on les met dans 
	une salle d'attente (Zone d'Index)
	
# [git status] permet de voir ce qu'on a ajouté
```

```github
git commit -m "explication"

# Crée un nouveau commit
# [git add] pousse les fichiers en zone d'index
# [git commit] les sauvegarde réellement dans un nouveau commit
```

---

##### <font color ="blueviolet">Tips</font>

>On peut faire un clic droit sur un dossier > ouvrir un *`git bash here`*
>Ouvre un terminal pointé sur le dossier sélectionné. 

```github
code .

# Ouvre l'application pour coder
```

> Après un *`git add .`* on peut vérifier ce que l'on a ajouté. Généralement on fait directement un commit, mais ça permet tout de même de se rendre compte de ce que l'on ajoute. 

```github
git status

On branch master
> No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   CheatSheet_GitHub.png
        new file:   index.html
        new file:   style.css
```



### <font color = "yellow">Gérer les commit (toujours en local)</font>
---

```github
git commit -m "Mon Message"

# Fait une sauvegarde et envoie dans un commit. 
	On peut faire un `git log` pour obtenir plus d'infos
```

![[Pasted image 20230723200739.png]]

> Là je fais un second commit pour visualiser les 2 commit qui ont été fait en faisant un  *`git log`*

![[Pasted image 20230723201635.png]]

##### <font color ="blueviolet">Tips</font>

>Si un jour on veut récupérer un commit spécifique, il suffit de copier la clé *`sha`* qui le concerne puis de taper la commande `git checkout` et coller la clé ciblée

> Pour coller : click molette

```github
git checkout dcd81f15ef4cb8d77e1f54aaa07ae96a168c2eb0
```

![[Pasted image 20230723203134.png]]

> On voit qu'on est passé du **master** au commit avec la clé concernée
> Dans notre éditeur de code, on peut se rendre compte que les fichiers ont changés avec la première version 

> Pour revenir sur la dernière version **master** : 

```github
git checkout master
```


### <font color = "yellow">Versionner en ligne (sauvegarder)</font>
---

Aller sur le profil **GitHub** puis créer un nouveau <font color="salmon">repository</font> et indiquer un nom
Copier le lien donné. Ex : https://github.com/fudev1/training-git.git

> Créer un clone d'un projet sur GitHub : 
> # ça va créer une copie du projet sur le pc (là où ouvrira le bash)

```github
git clone https://github.com/fudev1/training-git.git
```



