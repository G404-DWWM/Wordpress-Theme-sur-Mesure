# Wordpress & thème sur mesure

## 📺 Présentation

Qu'est ce qu'un child-theme ?

## 🎦 Live coding

Configuration d'un child-theme


## ⛳ Exercices

Installer un thème généré avec _s : [Underscores | A Starter Theme for WordPress](https://underscores.me/)

1️⃣ Installer l'extension **ACF** : [Advanced Custom Fields – Extension WordPress | WordPress.org](https://fr.wordpress.org/plugins/advanced-custom-fields/) .

A partir de l'instance Wordpress créée la veille :

* Créer un groupe de champs *Projets*
* Ajouter des champs dans votre groupe de la sorte (nom | type) :
    * titre | texte
    * description | éditeur WYSIWYG
    * URL | URL
    * image | image
    * date | date

2️⃣ **Créer le fichier** *content-project.php* à la racine de votre thème qui comportera :
la fonction PHP *get_fields*
les fonctions PHP de ACF nommées *the_field* qui permettront d’insérer chaque champ créé précédemment dans une balise HTML.
 Par exemple : ```<h1><?php the_field(‘nom_du_champ’); ?></h1>```

3️⃣ **Installer l'extension CPTUI** : [Custom Post Type UI – Extension WordPress | WordPress.org](https://fr.wordpress.org/plugins/custom-post-type-ui/)
* Ajouter un type de post, que vous nommerez *projet*
* Paramétrer le type de post de sorte qu'il prenne en compte les ACF
* Assigner le nouveau groupe de champ ACF à ce nouveau type de post

4️⃣ **Créer le fichier** *single-project.php* à la racine de votre thème
* Dupliquer le fichier *single.php*, le renommer en *single-project.php*
* Modifier le paramètre de la fonction PHP *get_template_part* par *content-project*

5️⃣ **Publier un nouveau projet !**
**🔥 Suite extra :**
* Ajouter les assets d'un framework de votre choix (Bootstrap / Material / etc.) au fichier *functions.php* grâce à la fonction PHP *wp_enqueue_script*
* Intégrer le reste des pages avec le DOM et CSS de votre framework d'intégration favori !

## Pour aller plus loin...
* [fr:Thèmes Enfant « WordPress Choodex](https://codex.wordpress.org/fr:Th%C3%A8mes_Enfant)
* [ACF | Resources, Documentation, API, How to & Tutorial Articles](https://www.advancedcustomfields.com/resources/)
* [3 façons d'utiliser Advanced Custom Fields pour WordPress](https://wpformation.com/advanced-custom-fields-wordpress/)
* [Combining Bootstrap with Underscores - Remejy . Com](https://remejy.com/combine-bootstrap-with-underscores/)

## 🏆 Objectifs
* Configurer et activer un child-theme
* Intégrer un thème sur mesure
* Configurer et utiliser ACF et les Custom Post Type

## 🧠 A retenir
* **A vos claviers !** ⌨️

