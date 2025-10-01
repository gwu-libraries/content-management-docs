---
description: Resources and information for OCLC's Connexion Client
---

# OCLC Connexion

## Fixing Diacritics Menu

With Windows 11, some Connexion users have reported that the Diacritics Menu is not synced up properly; it will show one diacritic but it is not the diacritic that gets inserted.&#x20;

1. Close **Connexion client** if it’s running.
2. Navigate to either **C:\Program Files (x86)\OCLC\Connexion\Program** (if using client 2.63) or **C:\Program Files\OCLC\Connexion\Program** (if using client 3.x)
3. Right-mouse click the **ALACOUR.TTF** file (this is the ALA BT Courier font) and choose **Install for all users.** If you don’t see the TTF extension, check the **Type** column for ‘TrueType font file’.
4. If you receive a message the ALA BT Courier font is already installed, answer **Yes** to replace it. If you're prompted for an administrator password or confirmation, type the password or provide confirmation.
   1. On GW owned machines, you have to right click on the file, select "Show more options" and then you'll find the "Install for all users" option.
5. Start Connexion client.
6. Display a record and bring the diacritics picker up. Everything should look normal.
