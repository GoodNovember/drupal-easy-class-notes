Class 4, Sept 4 2019

Continues Basic Intermediate data architecture

See previous class's video

Drupal Ladder (cool a few years ago)
http://drupalladder.org/

Hands on today! (yay!)

Entities. Bundles. Fields.

Entities API

Entity - read / write/ edit/ delete low level stuff
  Content Entity Base (see entity)
    Node
      Basic page
      Article
      Movie
    User
    Term (vocabularies)
      Tags
      Topics
    Comment (comment type)
    Block content (block content type)
    Message (cpmtemt fpr,) ???

NOTE:
  If you 'disable' the title of an entity, you will see an error because Drupal requires a title, even if it allows you to remove it.

  There exists an Auto_EntityLabel sort of thing that exists.

Default and Teaser are subtabs of Manage Display inside of Entity.

Each bundle can have defined and and configurable View Modes. By default, these are Default and Teaser.
Default is the fallback.
Teaser is like a summary for dislaying in a list, for example.

Custom Display Settings:
By default, there are 5 viewmodes for Node Entities
Full Content
RSS
Search Index
Search result highlighting input
Teaser

Display Modes
  Form Mode
    View the same Form in different ways.
  View Mode
    View entity's output
    Includes:
      Full Content
      RSS
      Search Index
      Search result highlighting input
      Teaser

In order to make an entity use a view, have a look at the entity's [Manage Display] mode's [Custom Display Settings]

---

Enabling Modules.

NOTE: 
  ddev exec [shell commands]
  ddev . [shell commands]

To enable an installed module, you can use:
  ddev . drush en [module_machine_name]