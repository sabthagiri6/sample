# GitHub Repo Template

GitHub Repo Template is a template for creation of open source projects made
available on GitHub. It includes a permissive open source license, a developer
certificate of origin, and a pull request template. This provides everything
necessary to have a properly licensed open source project.

## Using GitHub Repo Template

1. Clone or download this repository.
2. Copy its contents into your project (including the hidden .github directory). 
3. Customize each file to suit your project's needs (including the README). Look through the files for "TODO" and \<reponame\>, and replace with content appropriate to your project.
4. (Optional) Check out [GitHub Template Guidelines](https://github.com/cezaraugusto/github-template-guidelines) for ideas about how to customize your project.

TODO: describe a project in detail, what it does, how to use it, etc.

NI Package Manager Feeds
This repository contains NI Package Manager feeds for the plug-ins contained in MeasurementLink Plug-Ins Org.

Hosted Feeds
Feed Name	NI Package Manger Feed URL
all	https://raw.githubusercontent.com/NI-MeasurementLink-Plug-Ins/package-manager-feeds/main/package-feeds/all/Packages
Using Feeds in NI Package Manager
Once you subscribe to a feed, you will automatically gets updates as new releases are added to the feed.

Copy the NI Package Manager Feed URL from the Hosted Feeds table. This URL is the feed path.
Add the new feed in NIPM. Recommendation: Name the feed in NI Package Manager with something you will remember such as "GitHub MeasLink". Keep the name short because NI Package Manager does not keep a lot of visible space to display the name later.
Installing Packages from the Feed
Once the feed has been added in NIPM, you can install packages from this feed via the Packages tab.

Ensure that the Show available packages and feed management tools checkbox is checked in the NIPM settings. If unchecked, the Packages tab used below will not be shown. 
Select the Packages tab on the far right to show all packages that are available from the currently configured feeds, and search for your package from there.
Developers: Managing the Feeds
After creating a new release, you can add that release to a feed.

Adding New Packages to Existing Feed
To add a package to an existing feed:

Download the NI Package that you want to add to the feed to your development system.
Clone this repository and create a branch.
Use the Package Feed Updater Utility to add new package. Refer to Package Feed Updater readme for usage info.
Create a PR with the new package feed files (Packages, Packages.gz, and Packages.stamps).
Adding a New Feed
If you want to create a new feed (maybe to have a feed specific for a subset of packages), create a new folder under /package-feeds and use the Package Feed Updater Utility to create a new feed. Update the Hosted Feeds table with the new feed.

Recommendation is to add all new releases to the 'all' package feed.
