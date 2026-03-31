# OpenAthens Administration

#### Introduction

The OpenAthens admin console is available at [admin.openathens.net](http://admin.openathens.net). An Administrator account is required. Login is not connected to GW SSO, you have to create a password. This admin site is shared by Gelman and Himmelfarb. See also the OpenAthens documentation site at [docs.openathens.com](http://docs.openathens.com).&#x20;

We use the admin console for three types of functions: **user account administration**, **resource administration**, and **organization settings**. Most eresources staff only need the first two.

#### User Account Administration

Click the Accounts menu and select List to view user accounts. Ordinary user accounts are created automatically from GW SSO; these are listed under **George Washington University Library**. Alumni accounts also fall into this category. The other account types are created by staff. **Administrator** accounts are of course staff who have access to OpenAthens admin. **Access** accounts are created by staff for use of on-site visitors. These are generally created once per year and then reused, and are not limited to specific person or email address. Unlike other account types they are limited to on-campus IP addresses. Finally, **Personal** accounts are also created by staff but limited to a specific person or email address. We only create Personal accounts on rare occasions for testing purposes.

To check on a user account, you can search for a name, userid, or email address in the main OpenAthens account search box at the top. Note that if the same person falls into more than one category, you will see different information for that person in each column. &#x20;

#### Resource Administration

Within OpenAthens admin, sites or platforms that we have activated for access are called resources. There are two main types of resources: **federated** and **proxied**. There is also a third category called **custom** resources, which are a special type of federated resource. (Custom resources were called "go-live resources" during the OpenAthens implementation.)

* **Federated resources**: these create a direct connection between the provider and GW's SSO. We link to these resources with redirector links, and users can also log in at the resource itself.&#x20;
* **Proxied resources**: these work using a proxy server similar to our old EZproxy, but provided by OpenAthens. We link to these resources with redirector links. Most of these resources don't allow users to sign in at their site.
* **Custom resources**: these work with GW SSO, like federated resources, but each has its own unique setup behind the scenes. They generally have custom links instead of the usual OpenAthens redirector. Most also allow the user to sign in at the provider's site. This category is small but includes some of our biggest providers, such as ProQuest and Ebscohost.

You can see the the resources listed in OpenAthens admin by going to the Resources menu and selecting Catalogue. There are three lists. **Allocated** resources are those, both federated and proxied, that we have activated. **Custom** resources are all activated. **Available** resources include all those we have already activated, plus all federated resources that we have not activated, but NOT any proxied resources that we have not yet activated. In each list, the resources are shown with a blue "Allocated" button if already allocated, or a green "Allocate" button that you can use to allocate (activate) it. The blue and green buttons have a small drop-down menu where you can select the permission sets that can be used: default or alumni. Everything uses the default set except the resources specifically for alumni. (A third set, OSPO Zulip, is not used for library resources.)

#### Organization Settings

These are in the Preferences and Management menus. They include things like our Organization ID and the technical details for connecting OpenAthens to GW SSO. E-resources staff can view these settings, but should NOT edit them! If you have any questions about these settings, please see Matt Mihalik.&#x20;

<br>
