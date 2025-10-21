# Authentication and OpenAthens

**Introduction**

Authentication is the process of verifying to an eresource provider that someone is an authorized GW user. It is required for most paid online subscriptions and purchases. It is generally NOT required for free online resources.&#x20;

* The main authentication system for the GW Libraries is OpenAthens. We went live with OpenAthens in May 2024. Himmelfarb Health Sciences Library shares this system. Burns Law Library has a separate system, but law school users have full access to our OpenAthens.
* IP authentication is currently used as a backup. It will probably cease to be usable in the future, but we don't yet know when that will be. The GW VPN allows off-campus users to be authenticated by IP address.&#x20;
* Other authentication schemes, such as password access, are rarely used at GW and should be avoided unless there is no other option. The most important examples are our New York Times, Wall Street Journal, and Washington Post subscriptions.
* Our old authentication system, EZproxy, is no longer in use. URLs with our old base URL [proxygw.wrlc.org](http://proxygw.wrlc.org) are EZproxy links. Currently we have a system to redirect EZproxy links to OpenAthens, but this might not always be available. EZproxy links should be replaced with OpenAthens links wherever they are found.

**OpenAthens Overview**

OpenAthens is a system to manage single-signon (SSO) access to online resources. (The specific product we use is OpenAthens Compass.) In essence, our users authenticate to OpenAthens via GW SSO, and OpenAthens then authenticates them to eresource providers. The system is administered by the Serials & Eresources Group at Gelman, along with a team of librarians at Himmelfarb. Technical support is provided by ESCO, under contract. GW SSO is maintained by GW IT. Documentation is available at [docs.openathens.net](http://docs.openathens.net).&#x20;

Our OpenAthens ID is **81214475**. This is shared by Gelman and Himmelfarb. (There was originally a second ID specifically for Himmelfarb, 81242043, but this is no longer in use.)

Within OpenAthens, online resources fall into one of three categories: **federated**, **proxied**, or **custom**. The difference is mainly important for administration, but there are also some user-side differences between the three.

* Federated resources work fully with OpenAthens. We link to these resources with OpenAthens redirector links beginning [https://go.openathens.net/redirector/gwu.edu?url=](https://go.openathens.net/redirector/gwu.edu?url=) . Most of these resources also allow a user to sign in on their site, usually with a "Sign in through my institution" link.
* Proxied resources use a proxy server (similar to EZproxy) running inside of OpenAthens. We also use redirector links for these resources. Most of these resources will not allow users to sign into their sites directly.
* Custom resources (sometimes called "go-live" resources) have a special setup within OpenAthens. They usually have their own link schemes and do not use redirector links. They may or may not allow users to sign in directly on their sites. The most important custom resources are EBSCOhost, ProQuest, Ebook Central, Kanopy, O'Reilly eBooks, LinkedIn Learning, Digital Theatre+, and the Financial Times. New custom resources are rarely added. Almost all new resources are either federated or proxied.&#x20;

OpenAthens should work the same way whether the user is on or off campus. The user's location, and logging into the VPN, are usually only important when using IP Authentication.&#x20;

**OpenAthens URLs**

Most of our links to resources use the OpenAthens redirector scheme. A redirector link begins with the prefix [https://go.openathens.net/redirector/gwu.edu?url=](https://go.openathens.net/redirector/gwu.edu?url=) . After the "url=" comes an encoded version of the resource's URL. For example, https://muse.jhu.edu becomes  https%3A%2F%2Fmuse.jhu.edu%2F . With the redirector prefix, the complete URL would look like this:&#x20;

[https://go.openathens.net/redirector/gwu.edu?url=https%3A%2F%2Fmuse.jhu.edu%2F](https://go.openathens.net/redirector/gwu.edu?url=https%3A%2F%2Fmuse.jhu.edu%2F)&#x20;

Links formatted like this are called **Athenized** links. We have a tool to automatically Athenize links available on our LibGuide here: [https://libguides.gwu.edu/c.php?g=1397374\&p=10345898](https://libguides.gwu.edu/c.php?g=1397374\&p=10345898)&#x20;

**System Settings**: Links in our catalog, database list, and research guides can be Athenized automatically using these settings:

* Alma: Set "Proxy enabled" to Yes, and set "Proxy selected" to Default. (The default is OpenAthens, but choose Default instead of OpenAthens here so that we can manage all Default resources together.) Then put the original non-Athenized URL into the URL field (most resources activated from the CZ will already have it filled in). This setting is available at the Collection, Service, and Portfolio level. Some specific resources require special settings such as Parser Parameters.
* LibGuides, including the A-Z database list: set "Use proxy?" to Yes. Then enter the original non-Athenized URL into the URL field.&#x20;
* Primo Resource Recommender (managed within Alma): No setting. Copy the entire Athenized URL into the URL field. &#x20;

**IP Authentication**&#x20;

IP Authentication works by providers recognizing certain IP addresses as belonging to GW, and GW only allowing authorized users onto those addresses. These IPs include the GW wired and wifi networks and the VPN. In the future IP authentication may no longer work if, for example, the University starts obscuring users' IP addresses from providers. However, we do not yet know when changes like that will be made. For the time being, IP Authentication serves as a backup to OpenAthens, and as the main authentication method for a few resources that do not yet work with OpenAthens.

Our IP ranges are:

* 128.164.\*.\*  \[on campus and VPN]
* 161.253.\*.\*  \[on campus and VPN]
* 188.92.136.223  \[OpenAthens proxy server]
* 132.174.250.178 \[Burns Law Library's EZproxy server; add to subscriptions that we share with Burns]

188.92.136.238 was Himmelfarb's original OpenAthens proxy IP, before they combined accounts with LAI. This IP should be removed from our accounts as it may be reassigned to another OpenAthens institution.

198.91.37.2 was our old EZproxy server, and 198.91.37.66 was our old alumni proxy server. Any IP from the range 198.91.37.\* should be deleted from our accounts.

Usually we give our IP ranges to resource providers when we start a subscription. Many providers use the IP Registry ([theipregistry.org](http://theipregistry.org)) for IP updates. Our IP settings are already in the IP Registry, so in these cases we don't need to do anything else. GW's IP Registry admin is Ruth Bueter at Himmelfarb Library ([rbueter@gwu.edu](mailto:rbueter@gwu.edu)).&#x20;

Occasionally a provider may only be able to use one authentication system per account. In these cases we should choose OpenAthens instead of IP authentication, if possible. IP authentication is our second choice. Password access or anything else is our last choice. &#x20;

Some staff-side resources require an on-campus IP address: for example, the WRLC Service Desk. If off campus, sign into the GW VPN first.&#x20;

**Alumni and Visitor Access**

Both alumni and on-site guests are handled using OpenAthens. Note that logging into the GWguest wifi network does NOT automatically give access to library resources. &#x20;

* Alumni have access to certain specific online resources, listed here: [https://library.gwu.edu/info-for-alumni#eresources](https://library.gwu.edu/info-for-alumni#eresources). Clicking one of these links will authenticate the alumni user through OpenAthens. The user must have activated their account with GW Alumni first. Alumni who are visiting on-site can also use the procedure for visitors below for access to non-alumni resources.
* Visitors can request a guest OpenAthens login from the Access Desk. (They can get a guest computer/wifi login at the same time.) These logins are temporary and limited to on-campus IPs. Before using online resources, visitors should sign in with this login at [my.openathens.net](http://my.openathens.net) , using the option "Sign in with an OpenAthens account." Then they will be able to use Athenized links to our resources. See [https://library.gwu.edu/e-resource-access-visitors](https://library.gwu.edu/e-resource-access-visitors) for more information.
