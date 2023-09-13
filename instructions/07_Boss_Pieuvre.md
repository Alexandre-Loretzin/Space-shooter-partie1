# Boss fin de niveau 🐙🎮

## Apprition du boss

Pour faire apparaître le boss, nous allons surveiller la variable totalScore. Si elle dépasse 600, le boss fera son entrée. N'oublie pas de l'agrandir pour qu'il soit plus impressionnant ! 📈

![apparition du boss](images/apparitionBoss.png)

Il apparaît à droite et se déplace lentement vers la gauche. Une fois arrivé à destination, nous allons lui faire faire un mouvement de va-et-vient, de haut en bas, comme ceci :

![mouvement du boss](images/bossMouvement.png)

## Tir du boss

Le boss va tirer des projectiles vers le joueur. Pour cela, nous allons ajouter le comportement fireBullet à l'objet boss. Il tirera ses projectiles toutes les 0.6 secondes avec un multi fire de 5 et un firing arc de 35°. 🎯

![tir du boss](images/bossTir.png)

N'oublie pas de bien diriger le projectile vers le joueur et de faire en sorte qu'un projectile détruit le vaisseau du joueur. 💥

## Destruction du boss

On va attribuer une variable life au boss, comme pour les autres ennemis. On va lui mettre une valeur de 500 ! Ensuite, on va ajouter une condition qui vérifie si le boss est en collision avec un projectile. Si c'est le cas, on va décrémenter la variable life du boss. Si la variable life est inférieure ou égale à 0, on détruit le boss. 💔

![destruction du boss](images/boss_end_game.png)

Changeons le comportement des projectiles du joueur pour qu'ils affectent tous les ennemis et le boss. On peut les regrouper dans un groupe de scène, puis appliquer le comportement à ce groupe.

![projectiles](images/projectiles_enemies.png)

## Fin du niveau

Une fois le boss détruit, on va changer de scène pour passer à la scène suivante. On va aussi ajouter un écran de fin de niveau pour féliciter le joueur. 🏁

Je te laisse faire ça tout seul ! 🚀

## publication du jeu

La suite ici : [Publication du jeu](08_publication.md) 🎉
