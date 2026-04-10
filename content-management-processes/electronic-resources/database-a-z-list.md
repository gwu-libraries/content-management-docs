# Database A-Z List

#### Overview

Our main patron-facing database A-Z list is maintained in LibGuides. This gives us much more flexibility than the database records in Alma, and more features including integration with research guides. However, this does require us to maintain database records separately in both LibGuides and Alma. There is no automated connection between the two systems. Note that maintaining databases in Alma includes both the database collection records (not covered in this document) and the Primo database recommender (described below).

#### The Database List Public View

The public view of the database A-Z list can be seen at [https://libguides.gwu.edu/az/databases](https://libguides.gwu.edu/az/databases). Our Databases by Subject page is at [https://libguides.gwu.edu/databases](https://libguides.gwu.edu/databases) – see below for more. The most important elements of the A-Z list are:

* The alphabetical list by database title, which can be filtered by first letter
* The search box, allowing patrons to search by title or keyword in both the title and description
* The subjects filter, which uses a drop-down menu of predefined subjects
* Sidebar boxes, such as the Featured Databses box, which is permanent, and boxes for  New Databases and Test Databases, which only appear if those options are currently  enabled for one or more databases

There should be a description under each database title in the A-Z list. If the subject is longer than 600 characters, it will be truncated and there will be a View More link to show the full subject.&#x20;

We should make sure that every database record has a title, description, URL and proxy setting, and one or more subject areas. However, the title is the only element that is actually required by the system.

#### Managing the Database List

The A-Z list is managed in LibApps. All eresources staff should have an editor account in LibApps. Log in with SSO and select LibGuides from the app menu in the upper left. Then, from the Content menu, select A-Z List Management (new). Do NOT use the old version, "A-Z Database List," as it lacks some features that we use.

In the A-Z List Management screen, you'll see a list of all databases at the beginning, and you can search or filter using the fields to the right of the list. Note the "Mapping" column. This shows you the total number of research guides where that database has been shared or reused. Click on the number to get a list.

Database records are added using the Add Database button at the top. We do not use the Import Databases function. Existing databases can be edited by clicking the more options (three dots) button next to the database, and selecting Edit Database from the popup menu. This is also where you can delete a database. Finally, the Export Databases function can be used to make a backup copy or whenever you want to see our complete database in spreadsheet format.

To add a new database, click Add Database and fill in the fields below. In most cases the title, description, and subject tags will be specified by the ordering librarian, but in some cases you might need to do some research. Fields not listed here are optional.

1. Public Database Display: set to Show in AZ, unless we want to hide this database, in which case set it Hide in AZ
2. Database Landing Page: set to Inactive unless we have a specific need to add a landing page. (For an example, see Economist Intelligence Unit.)
3. Database Name: if the database has more than one possible name, we just have to pick one. If it starts with "The," leave that out. If there is a name in a non-Roman alphabet, you can include that in parentheses at the end of database name. &#x20;
4. Database URL: enter the basic URL with the initial "https" but without encoding and without the OpenAthens redirector
5. Use Proxy: set to Yes if we use the OpenAthens redirector with this database, or No if the database is not using OpenAthens, or if it has a custom OpenAthens URL without the redirector prefix
6. Database Description: Keep it under 600 characters if possible. May contain links. If a database requires the GW VPN for access, note that here.
7. Associated Subjects: select from the drop-down menu. This can be left blank in rare cases where none of the subjects fit.
8. Best Bets: currently NOT in use, but we may start using it in the future
9. Attributes: select these to put the database in the associated sidebar box; rarely used.
10. Additional Information: for databases that use a landing page, this is where the landing page fields are entered.
11. Each entry will also have an ID number that is generated automatically.

When editing an existing database, note that if you change the title, that may also change where the database appears in alphabetical list. In those cases, notify the owners of every research guide that reuses that database (see the Mapping column).

#### Database Subject Lists

The Databases by Subject page at [https://libguides.gwu.edu/databases](https://libguides.gwu.edu/databases) is actually a specialized research guide. This shows links to database lists for different subject areas, organized in a few overall categories. The subjects corresponds to the subject areas in each database record. However, there is no automatic connection. The subject lists, which are also research guides, have to be edited like any other research guide.

We do not normally make changes to the Databases by Subject landing page. However, we will edit it if we decide to change the subject categories we use in the A-Z list.&#x20;

The subject database lists can be found in LibGuides admin under Guides in the Content menu. You can recognize them because each has the word "Databases" at the beginning of the guide name, for example, "Databases: History."&#x20;

When we add a new database, the ordering librarian will usually specify the subject areas. Sometimes librarians also request that we add or change the subjects for a given database. To do this, go the subject guide in the list of guides and select Edit (the pencil icon). Most guides have both a Core Resources box, which is fixed, and an Additional Resources box, which is where all new databases go. At the bottom of the box, select Add / Reorder > Database. This will add the database at the bottom of that box. You then have to select Sort Database Group to put it in proper alphabetical order.&#x20;

#### The Primo Database Recommender

The Primo Database Recommender puts databases at the top of Primo search results, for greater visibilty for patrons. It is maintained in Alma, under Discovery > Resource Recommender Configuration > DATABASES. For the most part, we try to have a recommender entry for every database in the A-Z list. The recommender entry should be added AFTER you create the LibGuides A-Z list entry.&#x20;

To add a database to the recommender, go to the list in recommender admin, then click Add Resource. We do not use the "Add resources from electronic collections" function. You can also add or edit database entries using the Import command to upload a spreadsheet, but that is really only practical when making a large number of additions or changes at once.

The fields in database recommender entries are similar to those in A-Z list entries, but there are a few differences:

* Key: This should match the ID number in LibGuides. The system will automatically add "database" to the beginning of the number.&#x20;
* Name: Same as in LibGuides.
* Description: Same as in LibGuides, but here it is required that the description must be under 600 characters.
* Tags: Keywords that will bring up this entry when searched in Primo. Add as many as you think appropriate. Common abbreviations or alternate versions of the title are a good choice. You do not need to add all the subjects from LibGuides here. Each tag including the last one should be followed by a semicolon (;).
* Link: The complete link to the resource, including the OpenAthens redirector prefix and OpenAthens encoding. The most practical way to get this is to right-click and copy the link URL from the public view of the A-Z list.
* Link text: Enter "Go to database"
* Do NOT check the "Display Always" box.
