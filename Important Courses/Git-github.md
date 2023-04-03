Angela Yu!

# Git and local repositories

## Git init

- With this command we initialize git on a local repository. Which we initialize in the working directory of our preference.

```bash
git init
```

## Staging area

- An intermediate place where you can pick and choose which files inside your working area /directory that you want to commit

### To check what's in the stage area, untracked files

```bash
git status
```

### Adding to the staging area

- To start tracking changes on certain files, you need to add them to the staging area 
- You need to type the following:

```bash
git add andTheNameOfTheFile.txt
```

- If you use git status again you'll see that a file is the staging area and ready to be committed.

or

```bash
git add . 
```

	To add every file from the current directory. Everything inside the current directory.

## To commit all the files

- We use the following command:

```shell
git commit -m "a message"
```

### About commit messages

- You need to write them in present tense and be as precise as possible.

## Git log 

- You can see what changes you have committed using command.

```shell
git log
```


## Reverting a file

- Let's suposse you made a change you didn't want to. Well, that change probably hasn't been committed yet, the change is floating in git status waiting for you to take some action on it, be it adding it to the staging area or even commit it.

## Git diff

- We can use this command to compare what are the differences between the actual file and the last save point in our Git repository. 

```bash
git diff nameOfTheFile
```

## Rolling back to the previous version of a file

- It is important for you to note that you will only be doing this **just in case** you really want to roll back to your previous version of a specific file. 

```bash
git checkout nameOfTheFileYouWantToRollbackTo
```

# Github and remote repositories

## Creating a remote 

- The first step is to tell our local git that we've got some remote repositories over the internet and we add the following line of code:

```bash
git remote add origin https://github.com/Blisse1/MyObsidianVault.git
```

- Origin is just a theorical name, you can call it whatever you want, and the following instruction is the url of our github repository

- Once it has been created (the remote repository in our directory) we can now push our local repository onto our remote repository by simply typing:

```bash
git push -u origin main
```

- The -u option basically links up my remote and my local repositories
- Then we push to the remote repository that we previously called origin by convention
- and finally we'll be pushing it to a branch called in this case main or master
- The master branch is the default branch of all of our commits.

## To push an existing repository from the command line 

- En caso de querer actualizar con nuevos cambios y archivos nuestro repositorio remoto, simplemente añadimos los archivos por los pasos que hicimos antes con commit y luego hacemos un git push

## Para hacer una repo privada

- Cierta configuración de escribir y leer

## Permisos para repos privadas

- Solo darle permisos de escribir y leer a contents.

## Gitignore

- Just create a .gitignore file inside your working directory like so:

```bash
touch .gitignore
```


## Crear SSH

