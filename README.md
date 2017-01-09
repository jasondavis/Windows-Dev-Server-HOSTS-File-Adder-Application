# Windows HOSTS File Updater Build Tool
This WIndows Application allows a PHP script to call it and create a Windows HOSTS file entry for a Dev server domain.

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




























