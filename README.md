Welcome to your JBoss AS application on OpenShift
Deploying code changes
OpenShift uses the Git version control system for your source code, and grants you access to it via the Secure Shell (SSH) protocol. In order to upload and download code to your application you need to give us your public SSH key. You can upload it within the web console or install the RHC command line tool and run rhc setup to generate and upload your key automatically.

Working in your local Git repository
If you created your application from the command line and uploaded your SSH key, rhc will automatically download a copy of that source code repository (Git calls this 'cloning') to your local system.

If you created the application from the web console, you'll need to manually clone the repository to your local system. Copy the application's source code Git URL and then run:

$ git clone <git_url> <directory_to_create>

# Within your project directory
# Commit your changes and push to OpenShift

$ git commit -a -m 'Some commit message'
$ git push
Learn more about deploying and building your application
See the README file in your local application Git repository for more information on the options for deploying applications.
Sample Applications
To get started you can either modify the default war or try one of these samples:
kitchensink-example this quickstart showcases some of the exciting Java EE6 features available on JBoss AS 7.1.
kitchensink-html5-mobile-example based on kitchensink (above), but with an HTML5 client that displays great on a PC or mobile device.
tweetstream-example a TweetStream example
Example usage
cd kitchensink
git remote add upstream -m master git://github.com/openshift/kitchensink-example.git
git pull -s recursive -X theirs upstream master
Managing your application
Web Console
You can use the OpenShift web console to enable additional capabilities via cartridges, add collaborator access authorizations, designate custom domain aliases, and manage domain memberships.

Command Line Tools
Installing the OpenShift RHC client tools allows you complete control of your cloud environment. Read more on how to manage your application from the command line in our User Guide.

Development Resources
JBoss Developer Studio
The JBoss Developer Studio is a full featured IDE with OpenShift integration built in. It gives you the ability to create, edit and deploy applications without having to leave the IDE. Links to download, install and use the JBoss Developer Studio for Linux, Mac OS X, or Windows can be found on the JBoss Developer Studio tools page.

Debugging
View debugging information about the server environment including memory pools.

Getting Started with JBossAS on OpenShift
Developer Center
User Guide
Help Center
Stack Overflow questions for OpenShift
Git documentation