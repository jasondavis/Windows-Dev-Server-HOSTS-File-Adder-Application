# Windows HOSTS File Updater Build Tool
This WIndows Application allows a PHP script or any script for that matter to call it and create a Windows HOSTS file entry for a Dev server domain entry.  Useful in build scripts.

In addition to PH you could call the application from any type of langguage or build script.

The example below shows the basic usage to add a domain entry to my WIndows HOSTS file named `dev-project.dev`

Simply call the application `set-dev-server-domain-hosts-file-entry.exe` followed by a space and then the name of the desired DOmain name to add to the HOSTS file.

## Usage

    // Add record to Windows HOSTS file
    // HOSTS file C:\Windows\System32\drivers\etc\HOSTS
    @exec('set-dev-server-domain-hosts-file-entry.exe dev-project.dev');

## Whats Included

- The WIndows EXE Application `set-dev-server-domain-hosts-file-entry.exe`
- A `demo.php` PHP test file to show usage in PHP
- A shortcut to view the HOSTS file in WIndows 7 and possibbly other WIndows versions.
- This `README.md` file to explain the library and show how to use it.
- `Windows-Dev-Server-HOSTS-FIle-PHP-Updater-Library.zip` ZIP archive containing all the files in this library.

## Why?
I use this on my localhost dev server with a PHP script to quickly create new projects.  A project does the following:

- Uses this library to update my Windows HOSTS file with a new Dev server domain name for the project
- Creates a MySQL Database server if I tell it for the project.
- Creates a folder in my dev server which has an APache virtualhost config to make the new Dev server domain work with the new roject folder.
- Otionally download and install a WordPress app, a Laravel App, or a SUgarCRM app on the Project.
- More to come soon

## Localhost Dev Server Project Build Script Plans:

Eventually I will release my PHP Project creation script with this library and add new features to it.

In addition to a Projects folder on my Localhost Dev server I also have a Labs folder which I use to install and test PHP and JS libraries I come across and like online as well as create simple JS and PHP test lab projects.

I would like to add my Labs to my Project creation script with some of these features planned:

- Option to enter a GitHub repo and have it clone the repo into the Lab project
- Use Composer for some PHP projects
- Option to create a JSBin, CodePen.io, JSFiddle, and more projects.
- Store each LAb project in a MySQL DB or an SQLite DB and then have a Listing page to view all my Lab Projects in a list with name, description, demo URLs, project URLs, and preview images.
- Same as above but DB entries for the Projects directory.

## Request For your Dev Server Build Script Feature Ideas
Please feel free to create an Issue on this repo with any ideas you might have for this build script and new features.








































