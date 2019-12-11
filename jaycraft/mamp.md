# Use with MAMP

At this stage, JayCraft is built for use with MAMP Pro. Below are some features of JayCraft to optimise it for developing a CraftCMS project with MAMP.

As setting up SSL on MAMP is usually done once per project, it can be a while between each set up, making it easy to forget the process. Below is how I do it for my projects.

> These docs are mostly for myself instead of Googling how to do it and finding the same StackOverflow questions.

## SSL 

As our live sites should be SSL protected by default, it's good to develop in a faux-secure environment so our local and staging/production servers are as similar as possible.

Firstly, you need to set up your [SSL certificate within MAMP](https://documentation.mamp.info/en/MAMP-PRO-Mac/Settings/Hosts/SSL/)

Once you have an SSL certificate for your project we need to tell our computer that it is safe even though it is 'self-signed'. I do this on my Mac like this:

1. Open Keychain Access on your Mac
2. Find the relevant SSL certificate for your project and select it
3. Expand the "Trust" tab within this window
4. Select "Always Trust" from the top option labelled "When using this certificate"

Now your Mac won't have a panic attack when you open your local site with `https://`.

> Note that you should check the "Allow HTTP connections" checkbox at the bottom of the SSL panel in MAMP to keep the non-HTTPS version of the site working.

## Database backups

As CraftCMS as of version 3 uses the `mysqldump` command to dump the database (when requested via the CLI or within the CMS), database backups won't work with MAMP.

CraftCMS document the method how to configure your projects to [work with MAMP](https://craftcms.com/guides/database-backups-in-craft-3-with-mamp) by adding `BACKUP_COMMAND` and `RESTORE_COMMAND` commands to the .env and general config files.