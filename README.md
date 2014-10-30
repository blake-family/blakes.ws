http://www.shaunblake.com
=========

Website project and distribution for http://www.shaunblake.com

The site is hosted as github pages.  The project uses yeomen, grunt, and bower. The site itself uses polymer.

##deploying
The site is contained on the gh-pages branch and found in the dist directory. Deployment is handled by a handy script I found (and checked in at the root) - https://github.com/X1011/git-directory-deploy

`./deploy` will push the dist folder up the github as the new site (use `./deploy -s` the first time???).

##Custom Domain

###DNS Configuration
I have two @ A name records, 1 pointing to 192.30.252.153 and one pointing to 192.30.252.154.  Then I have a www A name record pointing to 192.30.252.153.

###Github configuration
I have the previously mentioned deploy script which will deploy the dist version to the gh-pages branch.  In the root I have a file, CNAME, which has www.shaunblake.com.  Including the www means shaunblake.com will redirect to www.shaunblake.com. If I just had shaunblake.com then www.shaunblake.com would redirect to shaunblake.com.
