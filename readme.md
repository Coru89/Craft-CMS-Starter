You can start using DDEV with an existing project, too—just make sure you have a database backup handy!

# Clone an existing repository (or navigate to a local project directory):
git clone https://github.com/example/example-site my-craft-project
cd my-craft-project

# Set up the DDEV environment:
ddev config --project-type=craftcms

# Boot the project and install Composer packages:
ddev start
ddev composer install

# Import a database backup and open the site in your browser:
# Corey: MUST IMPORT A DB!! Can use the db-for-import.sql.zip at root
ddev import-db --src=/path/to/db.sql.gz
ddev launch