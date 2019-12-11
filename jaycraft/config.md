# Config

When starting a new project with JayCraft, these are the project-specific configuration options you need to review:

## .htaccess

The project `.htaccess` file within the `/public` directory has three key features:

1. Craft's own 404 request handler
2. Fortrabbit app URL redirect (I host with [Fortrabbit](/hosting.md))
3. HTTPS redirects

The first takes care of itself and has nothing specific to your project.

However, the second and third will both need a URL modified to reflect your project.

## .env

The `.env` should be configured when you boot up JayCraft, but once you're up and running you will need to edit the `DEFAULT_SITE_URL` rule to reflect your local build URL.

This setting is set to the following by default:

```
DEFAULT_SITE_URL="https://local.jaycraft.com"
```

## /public _not_ /web

I prefer to develop inside a `/public` directory instead of CraftCMS' default, which is `/web`.

So, JayCraft will be setup with a `/public` directory! This is important to remember when configuring your staging/live servers.