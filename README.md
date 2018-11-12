# Tuto Reaveal.js

Lien vers le diapo pour voir ce qui est possible :arrow_forward: [Diaporama](https://healermikado.github.io/prensentationRevealJs/#/)


Lien vers le github de reveal.js qui est très complete :arrow_forward: [reaveal](https://github.com/hakimel/reveal.js/)

## Pourquoi utiliser reveal.js ?

WIP

## Comment utiliser reveal.js ?

1. Télécharger le contenu du dépôt https://github.com/hakimel/reveal.js/
2. Modifier le conten du fichier index.html avec un éditeur de code (visual studio code fonctionne bien)
3. Pour voir sa présentation ouvrir avec un navigateur internet le fichier index.html

## Comment faire sa présentaton

Voici le point le plus important de ce tuto, comment écrire votre présentation. Reveal.js est un framework html/css/javascript. Pour écrire une présentation vous allez écrire du code HTML (mais promis c'est facile).

### Faire une slide

Pour faire une slide vous allez créer une balise <section>.

```HTML
<section>
    code de ma slide
</section>
```

Reaveal.js permet également de faire des slides imbriquées (très utile pour développé une idée). Cela donne quelque chose comme ça

```HTML
<section>
    <section>
        slide 1
    </section>
    <section>
        slide 2
    </section>
</section>
```

Vous ne pouvez pas faire plus d'un niveau d'imbrication

### Contenu d'une slide

#### Les titres

Pour faire le titre de la slide vous avez à votre disposition les balises h1, h2, h3, h4, h5, h6. h1 étant le titre le plus forte, et h6 le plus faible. Dans les fait j'utilise rarement plus que du h3. Souvent voilà ma hiérarchie des titres

1. h1 : titre du diapo (donc uniquement sur ma première slide)
2. h2 : titre d'une partie
3. h3 : titre d'une slide

Exemple :

```HTML
<section>
    <h1>Ma super présentation</h1>
</section>
<section>
    <section>
        <h2>Ma super partie 1</h2>
    </section>
    <section>
        <h3> Ma super slide 1 </h3>
    </section>
    <section>
        <h3> Ma super slide 2 </h3>
    </section>
</section>
<section>
    <section>
        <h2>Ma super partie 2</h2>
    </section>
    <section>
        <h3> Ma super slide 3 </h3>
    </section>
    <section>
        <h3> Ma super slide 4 </h3>
    </section>
</section>
```

#### Les paragraphes

```HTML
<p> mon super paragraphe </p>
<p> mon paragraphe trop bien </p>
```

ou sans balise et en sautant des lignes.

```HTML
 mon super paragraphe 

 mon paragraphe trop bien
```

Pour du text en gras :

```HTML
<b> important </b>
```

Pour du text en italique :

```HTML
<em> important </em>
```

#### Les listes

C'est comme les listes en html. On peut faire des listes ordonnées (ol>li) ou non ordonnées (ul>li)

``` HTML
<ol>
    <li> elem 1</li>
    <li> elem 2</li>
    <li> elem 3</li>
    <li> elem 4</li>
    <li> elem 4</li>
    <li> elem 5</li>
</ol>

<ul>
    <li> elem 1</li>
    <li> elem 2</li>
    <li> elem 3</li>
    <li> elem 4</li>
    <li> elem 4</li>
    <li> elem 5</li>
</ul>
```

#### Les tableaux

```HTML
<table>
    <thead>
        <tr>
            <th>Item</th>
            <th>Value</th>
            <th>Quantity</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Apples</td>
            <td>$1</td>
            <td>7</td>
        </tr>
        <tr>
            <td>Lemonade</td>
            <td>$2</td>
            <td>18</td>
        </tr>
        <tr>
            <td>Bread</td>
            <td>$3</td>
            <td>2</td>
        </tr>
    </tbody>
</table>
```

#### Les images

```HTML
<img src="chemin/vers/image" alt="" class="plain"/>
```
