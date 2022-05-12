`xss injection`
> sur la page [feedback](http://192.168.1.143/index.php?page=feedback), on ecrit juste ***alert*** ou ***script*** pour pouvoir créer une faille XSS.
`Comment éviter la faille`
> filtrer les input avec les fonctions *SANITIZING* afin d'eviter les mots clés et les caracteres spéciaux.
```
htmlspecialchars 
```