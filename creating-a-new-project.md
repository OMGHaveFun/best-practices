# Creating a New Project

* [Choosing the shortname (and everything-name) of your project](#gshortname)
* [Creating the project from our client-boilerplate](#client-boilerplate)
* [Forking a project to start a "2.0 version" while 1.0 or the "one-pager" lives on](#g2)

## <a name="gshortname">Choosing the shortname (and everything-name) of your project</a>

The "shortname" of your project, like "ccd" or "pogil" or "thenotebook", must also be the name of the repo, the name of the database, the name of the directory on the server (and on your hard drive), and the name of everything else that requires a unique name for the project. Do everything you can to avoid diverging on this point.

The shortname may contain lowercase letters, digits, and hyphens. Nothing else.

The shortname should be short, but consistency is even more important than brevity.

## <a name="client-boilerplate">Creating the project from our client-boilerplate</a>

We have a `client-boilerplate` project which is designed to be used with the Apostrophe CLI
to create a project that is set up for our best internal practices.

Do not use the default `apostrophe-boilerplate`. Instead, type:

```
# If you didn't already, install the CLI
npm install -g apostrophe-cli

# Now make your project
apostrophe create-project YOUR-SHORTNAME-HERE --boilerplate=https://github.com/punkave/client-boilerplate
```

## <a name="g2">Forking a project to start a "2.0 version" while "1.0" lives on</a>

**If a project is "forked," for instance to create a full site from a placeholder site, and the placeholder site continues to be live in the meantime, the shortname / database name / everything name must be different for the fork.** This avoids ugliness when we inevitably want to deploy the new site side by side with the old during a transitional period as new content is created.

A common example is a case that begins life as a "one-pager" and then goes into development as a larger site. They must coexist temporarily and the customer will want to use the same server to manage costs. If there is any risk of the database name being the same, bad things can happen.


