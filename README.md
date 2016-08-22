## Jelastic Git-Push-Deploy Add-on 

This repository provides an example of automated CI with public git repository integration w/o authentication.

### What it can be used for?

With a help of this JPS add-on, Git-Push-Deploy is installed on app server available in the environment to provide possibility to connect and update the project in automatic mode from Git repository after changes pushed.

[![Git-Push-Deploy](https://docs.google.com/drawings/d/1nTTTYGob9r3Hkb3tDytg9ZTPSeGjVzxhV4jR0p2G9TA/pub?w=512&h=319)](../../../git-push-deploy)

### How To Use

**Fork and customize**: 
- Update the link to your public git repository in the [manifest](manifest.jps).
- Modify "post-merge" hook for custom actions inside "after-deploy-hook" procedure in the same manifest.
- Change aplication server or entire topology inside "topology" section in the manifest.

---

### Deployment

In order to get this solution instantly deployed, click the "Deploy" button and press Install.

[![Deploy](https://github.com/amoruga/git-push-deploy/raw/w/o-auth/images/deploy-button.png)](http://app.devops.virtuozzo.com//?manifest=https%3A%2F%2Fgithub.com%2Famoruga%2Fgit-push-deploy%2Fraw%2Fw/o-auth%2Fmanifest.jps)

To deploy this package to Jelastic Private Cloud, import [this JPS manifest](../../raw/w/o-auth/manifest.jps) within your dashboard ([detailed instruction](https://docs.jelastic.com/environment-export-import#import)).

For more information on what Jelastic add-on is and how to apply it, follow the [Jelastic Add-ons](https://github.com/jelastic-jps/jpswiki/wiki/Jelastic-Addons) reference.
