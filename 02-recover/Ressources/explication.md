`recover`
> qund on veux recuperer un mot de passe perdu sur la page [I forgot my password](http://192.168.1.143/?page=recover)
> on a pas de formulaire pour entrer l'adresse mail et on a un bouton *submit* tous seul, ce qui est bizard 

> En inspectant la page, on peut voir dans le form que il y a un *input* avec *mail* qui contient une adresse mail en dur.

```
<form action="#" method="POST">
	<input type="hidden" name="mail" value="webmaster@borntosec.com" maxlength="15">
	<input type="submit" name="Submit" value="Submit">
</form>
```

>Le bouton *submit* permet d'envoyer un mail à "webmaster@borntosec.com", en changeant ce mail on récupère le flag.

>Cette faille pourrait permettre d'envoyer un mail en provenance du site à n'importe qui.

`Comment éviter la faille`
> pour eviter cette faille, il suffit de gerer le *mot de passe oublier* en back-end