# Projey Site Statique

## Manuel

### 1

Pour commencer placer vos fichiers markdown ainsi que les images dans le dossier Markdown et renommer les markdown1.md, markdown2.md etc.. ( gére fichier markdown robuste )

```
PS C:\Users\Desktop\convertMdToHtml> ls
    Répertoire : C:\Users\Desktop\convertMdToHtml


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----       16/01/2019     15:22               ** Markdown **
d-----       16/01/2019     14:53                sitestatique
d-----       16/01/2019     13:50                template
-a----       16/01/2019     15:27           2226 convert_md.py


```
```
PS C:\Users\Desktop\convertMdToHtml\Markdown> ls
    Répertoire : C:\Users\Desktop\convertMdToHtml\Markdown


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----       16/01/2019     15:21          12989 logo.png
-a----       16/01/2019     15:26            328 ** markdown1.md **

```


### 2

Ensuite executer le programme qui convertira le fichier markdown en html/css avec ou sans les parametres d'execution
```
PS C:\Users\Desktop\convertMdToHtml> python .\convert_md.py
```
ou
```
PS C:\Users\Desktop\convertMdToHtml\sitestatique\HTML> python .\convert_md.py -i .\Markdown\ -o .\sitestatique\
```
* Le -i ou --input-directory vous permez de choisir le dossier avec le fichier markdown
* Le -o ou --output-directory servent à choisir le dossier ou vous trouverez les fichier css et html


### 3

Et vous trouverez les fichiers index.html et index.css dans le dossier sitestatique 
```
PS C:\Users\Desktop\convertMdToHtml\sitestatique> ls
    Répertoire : C:\Users\Desktop\convertMdToHtml\sitestatique


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----       16/01/2019     13:48                CSS
d-----       16/01/2019     15:25                HTML


PS C:\Users\Desktop\convertMdToHtml\sitestatique> cd .\CSS\
PS C:\Users\Desktop\convertMdToHtml\sitestatique\CSS> ls
    Répertoire : C:\Users\Desktop\convertMdToHtml\sitestatique\CSS


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----       16/01/2019     15:49           1342 ** index.css **


PS C:\Users\Desktop\convertMdToHtml\sitestatique\CSS> cd ..
PS C:\Users\Desktop\convertMdToHtml\sitestatique> cd .\HTML\
PS C:\Users\Desktop\convertMdToHtml\sitestatique\HTML> ls
    Répertoire : C:\Users\Desktop\convertMdToHtml\sitestatique\HTML


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----       16/01/2019     15:49            895 ** index.html **

```

# 4

Vous pouvez modifier le css ainsi que le header et le footer html de vos pages en modifiant les fichiers basecss.txt, basehtml.txt et fin_html.txt dans le dossier template.

