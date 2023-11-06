## CCA Rights

**Deprecated - please install from https://www.drupal.org/project/cca_rights**

A Drupal 9/10 feature module that creates a CCA Rights taxonomy and uses Migrate framework to generate some Creative Commons and Rights Statements.org licenses as taxonomy terms. Includes a field formatter to show CC icons with CC license URLs.

* Enable module
* Import terms
  * drush migrate:import creativecommons_rights_term --userid=1 --uri=http://{your site domain}
  * drush migrate:import rightsstatements_rights_term --userid=1 --uri=http://{your site domain}

Change Repository Item or other content types to add an Entity Reference field that matches against Rights vocabulary.

You may want to create your own entity reference view that hides unpublished terms. Then unpublish any imported rights terms that are not applicable to your content.
