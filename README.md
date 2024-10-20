## Project setup
To set up the project, follow the steps below:
1. Install DDEV on your machine. You can find the installation instructions [here](https://ddev.readthedocs.io/en/stable/#installation).
2. Clone the project repository to your local machine.
3. Navigate to the project directory and run the following command to start the project: ```ddev start```
4. Run the following command to import the database: ```ddev import-db --src=dbs/dump.sql.gz```
5. Run the following command to import configuration: ```ddev deploy -y```
6. You can start working on the project by visiting the URL: ```http://drupal-sandbox.ddev.site```
7. You can access the admin panel by visiting the URL: ```http://drupal-sandbox.ddev.site/user/login``` ```username: admin``` ```password: admin```

## DDEV commands
Here are some useful DDEV commands that you can use to manage the project:
1. ```ddev start``` - Start the project.
2. ```ddev stop``` - Stop the project.
3. ```ddev restart``` - Restart the project.
4. ```ddev auth ssh``` - SSH into the project.
5. ```ddev exec``` - Execute a command in the project.
6. ```ddev import-db --src=./dbs/db.sql``` - Import the database.
7. ```ddev deploy -y``` - Import configuration and update database.
8. ```ddev cex -y``` - Export all configs to file.
9. ```ddev cim -y``` - Import all configs from file.
10. ```ddev db-pull``` - Pull database from dev env to local.
11. ```ddev db-push``` - Push database from local env to the remote (dev).
12. ```ddev poweroff``` - Stop the project and free up resources. Use this command when you are disable DDEV and can work on other projects and systems on Docker.
13. ```ddev xdebug``` - Enable xdebug. Required file mapping in PHPStorm.
14. ```ddev ssh``` - SSH into the project in Docker container.
15. ```ddev composer <command>``` - Run composer commands in the project.
16. ```ddev drush <command>``` - Run drush commands in the project.

## Development workflow
The project follows a simple development workflow that involves the following steps:
1. Make sure to keep the project up-to-date with the latest changes from the main branch.
2. Create a new branch from the main branch.
3. Make changes to the code.
4. Commit the changes to the branch.
5. Push the branch to the remote repository.
6. Create a pull request to merge the branch into the main branch.
7. Ask for review the pull request by another Dev/Lead and merge it into the main branch.
8. Delete the branch after merging.
9. Repeat the process for new features or bug fixes.
