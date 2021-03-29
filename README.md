# Registering a Domain

Route 53 is AWS's DNS service.

It allows you to register doamins, so it can bill you and get a domain added \
to a generic TLD (Top-Level Domain), or a country code TLD registry. \
It also provides the ability to host the zone for your domain, \
and it provides managed Nameservers, which actually host that domain on your behalf.

Route 53 offers an end-to-end DNS service!

\
**Register a Domain:** \
Route 53 → Domains → Registered Domains → Register Domain

Domain Name: example \
Extension: Each of these have different annual prices (ex: .com - $12; .net - $11; .io - $39; .click - $5; .movie - $306) \
Check: see if example.com is available! If it's not available, view all the alternative suggested options below. \
Add to Cart \
Continue

Contact Information: \
Registrant Contact: person that is aware that the domain is being registered, and can answer queries in that context \
Technical Contact: person that can assist technically \
Admin Contact: person who is aware of the admin side of things (billing & renewal)

You can have the option selected \
that the Registrant, Technical, and Admin Contacts are all the same, \
and whether or not to hide some contact details (Privacy Protection).

Continue

Enable/Disable Auto-Renewal of your Domain\
Check box to agree to Terms and Conditions\
Complete Order

\
Now, AWS is communicating with the .org registry (or whatever extension you chose). This organization is known as PIR (Public Interest Registry). \
The first step is to get the example.org domain added to the zone file for .org (PIR controls this). \

Route 53 → Domains → Pending Requests \
Notice the status is "Domain registration in progress". We are waiting for this entry to be added to the .org zone file!



