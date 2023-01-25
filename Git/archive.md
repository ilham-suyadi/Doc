# Git Archive

```sh
git archive --output=./git.zip --format=zip head
atau
git archive --output=./git.zip head
```

> *git archive* = basic command
> *--output*    = akan memberi nama file hasil ekstarkannya
> *--format*    = ini akan memberitahu format yang akan di gunakan
> *head*        = versi yang akan di compres

## Mengkompres forder git tertentu

```sh
git archive --output=../git.zip head ./Git
```

> *./Git*       = folder yang akan kita compress

</br>

> :link: Refrensi : <https://www.atlassian.com/git/tutorials/export-git-archive>
