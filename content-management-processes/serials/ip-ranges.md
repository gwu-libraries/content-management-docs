# IP Ranges

IP authentication is still available at least through Spring 2026. All providers should be given our IP ranges. However, some providers will no longer support IP authentication after we've started using OpenAthens with them.&#x20;

* Our main IP ranges are: **128.164.\*.\*** and **161.253.\*.\***
  * these are both on campus and on the VPN
* OpenAthens proxy IP: **188.92.136.223**
* Burns Law Library's EZproxy server: **132.174.250.178**
  * add this to subscriptions Burns might want to add to their proxy server, or whenever Burns requests it
* Our IPv6 ranges: **2606:69C0::/32** and **2620:106:C000::/44**
* IP ranges not in use that should be deleted:
  * 188.92.136.238 (Himmelfarb's old OpenAthens proxy)
  * 164.82.22.0-127 (GWU Hospital. This is considered off-campus. Himmelfarb has it on a few subscriptions, but Gelman does not use it.)
  * 198.91.37.2, or anything in the 198.91.37.\* range (our old EZproxy servers)
  * 216.147.\*.\*, 74.82.\*_.\*,_ and 204.168.\*_.\*_ (other old systems we no longer use)
