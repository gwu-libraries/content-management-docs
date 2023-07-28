# API Setup

## Alma Integration

MarcEdit and Alma Integration (20180716rev)

Set up ILS integration to Alma. Click on < ![](<../../.gitbook/assets/image (3) (1).png>)> on lower right corner of main menu.

![](<../../.gitbook/assets/image (6) (1).png>)

&#x20;

Select \<ILS Integration> to begin setting access to Alma

![](<../../.gitbook/assets/image (4) (1) (1).png>)

&#x20;

Set up access to Alma as default:

&#x20;

Host name: [https://api-na.hosted.exlibrisgroup.com](https://api-na.hosted.exlibrisgroup.com)

Password: <\<PLEASE SEE MATTHEW BRIGHT FOR PASSWORD>>

&#x20;![](<../../.gitbook/assets/image (5).png>)



&#x20;![](<../../.gitbook/assets/image (2) (1).png>)\


Edit setting of Z39.50:

The character set in Alma is UTF-8

&#x20;

(Voyager setting was MARC-8)

&#x20;![](<../../.gitbook/assets/image (8) (1).png>)

&#x20;

Now that the ME to Alma integration has been established, the \<Alma> tab on MarcEditor tool is active and ready for searching, update/create MARC records in Alma via Z39.50.

![The appropriate menu in MarcEdit.](../../.gitbook/assets/Untitled.png)



The \<Search> function utilizes Z39.50 Bib1 attribute document for the specific indexes. Here are the basic search indexes available in Marcedit version 7.



&#x20;

Consult the Bulk\* search documents on best strategies on batch searches on other fields, especially \<Raw (Adv.)> search.

&#x20;

Pre-process of MARC data is available under \<Process Settings>.  This function calls the Tasks that have already been established.



To create Tasks anew, from \<Tools>, select \<Manage Tasks>--\<Create New Task List>--enter name of this new task list.





An example of various tasks added to a Task list below.

&#x20;

Related documents:

Alma APIs [https://developers.exlibrisgroup.com/alma/apis/bibs](https://developers.exlibrisgroup.com/alma/apis/bibs)

MarcEdit takes advantage of:

&#x20;   /almaws/v1/bibs

&#x20;       Create Record

&#x20;       Update Record

&#x20;       Retrieve Holdings List

&#x20;       Create Holdings List

&#x20;       Update Holdings list





## OCLC Integration
