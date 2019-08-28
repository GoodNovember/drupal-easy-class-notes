Q: Proxy Files? --- ask mike about doing this instead of inflating a zip file in ddev.


Composer Templates?

Keep composer min stability to be 'stable' unless you need something special

How do you find a vendor/library pair?
Packagist.org

Drupal:
Not best practice:
  Downloading Tarball

Best Practice:
  use "drupal-composer/drupal-project"

  We use a composer template because by default Composer will just
  dump everything into the vendor folder.

  The template allows us to put the required files where they want.

  drupal-project scaffolds our code using some handly libraries.

  Explore composer.json like package.json


---

This is how Mike likes it.

make a directory

```
mkdir dcoweek1
cd dcoweek1
```

Do some tweaks: (soon to be best practice)

```
ddev config
ddev start
```

that sets up a blank DDEV container with php type project.

Next, SSH into the web container.

```
ddev ssh
```

... see docs ... :-( there were problems.

---

Big 5

Entities
  php object that contians properties and methods.
    content-type -- can add fields

      Movie
        title [text]
        boxOfficeGross [number]
        director[s] [array of strings]
        releaseYear [date]
        rating [number]

  There can be different kinds of entity
[Entities]
  [Content Entites]
    [content-type] -- bundles
      - articles -- bundle
        - [fields]
      - basic pages -- bundle
        - [fields]
  [Taxonomy Entities]
    [Vocabularies] -- bundles
      - tags -- bundle
        - [fields]
  [Block Entites]
    [block-type]
      - basic block
        - [fields]
  [User entity]
    !! no bundles !!
    There is only one kind of user by default.
      - [fields]

---

Migration
  What are three things that you like and what are 3 things that you dont't like about the current website.

Get the content filler iner in front of the screen to test out the IA before theming begins.

