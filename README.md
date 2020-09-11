# "declarebusinessgroup" virus cleaner script

## Make a backup before running this script.

### What this script does:

-   Iterates over all current directories and subdirectories looking for targeted files (.js*. .htm*, .ph\*)
-   Finds dirty code and removes it
-   Changes targeted file permissions back to a safe value (0644)
-   Lets you know how many files were cleaned

### What it doesn't do:

-   Clean the database

I made this script to clean a targeted website I was working on. Fortunately the (poorly written) malware
did not succeed in changing the databse, so there's no code here for that, but it shouldn't be hard to do on a single
sql command.

Instructions:

-   Drop this file in your website's root directory
-   Run it, either by visiting "your_website.com/malware_cleaner.php" or runing "php -f" on it

Beware that this script will set permissions for targeted files to 644, so if you had files
with custom permissions before the infection, remember to change them. But for most people, just
running on your website's root directory should clean it.
