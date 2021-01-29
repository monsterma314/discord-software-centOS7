Source: https://dl.discordapp.net/apps/linux/{version}/{name}-{version}.tar.gz

**Step 1: Download the .tar.gz (Example Uses 0.0.11)**

The proper URL for the .tar.gz download of version 0.0.11 is:

	https://dl.discordapp.net/apps/linux/0.0.11/discord-0.0.11.tar.gz

**Step 2: Extract the Files in the Directory of Choice**

I put the files in my ~/Software directory (/opt is also common)

	   $ tar -xvf discord-0.0.11.tar.gz
	   $ cd Discord


**Step 3: Change the ~/Software/Discord/resources/build_info.json File**
   Since Discord will force an update to the newest version (via clean reinstall) 
   if you just start it up, you must fake the latest version. Replace the version
   variable in build_info.json using your favorite editor:

   $ emacs ~/Software/Discord/resources/build_info.json # Since recent version is 0.0.13, I used version 0.0.13

**Step 4: Install and Run Discord**

	$ sh ~/Software/Discord/Discord # will install modules in ~/.config/discord by default and run

***References***

Version Number edit: https://www.reddit.com/r/discordapp/comments/iqc0b9/to_all_the_folks_on_linux_who_cannot_update_nor/