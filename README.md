# Magento 2 .gitignore

Magento 2 projects don't have to live in a VCS root in it's entirety. While the dependency upon third-party hosting services is a valid point, it has to be solved in a different way.

To capture all moving parts of a shop, I use the following .gitignore file. 

# Hints

You can simply install Magento 2 in any given way. With this .gitignore file everything is ignored, except:

* config files with .dist file extensions in app/etc, so you can provide meaningfull templates for the deployment
* app/code
* app/design/frontend/<themename>
* composer.lock & .json  
* the .gitignore file itself
  
You most probably only have to take a look at the line where the theme package is whitelisted.
