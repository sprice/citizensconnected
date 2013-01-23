Citizens Connected Drupal distribution
======================================

This is the Drupal 7 distribution for Citizens Connected.

To Build & Install
------------------

To build a fresh install (full Drupal core + profile) for development,
run the following commands:

    mkdir -p public_html/profiles
    git clone https://github.com/sprice/citizensconnected.git public_html/profiles/citizensconnected
    cd public_html
    drush make --prepare-install profiles/citizensconnected/build-citizensconnected.make --yes
    drush -y site-install citizensconnected --db-url=mysql://user:pass@localhost/db_name --site-name="Site Name" --account-name=admin --account-pass=[password]
