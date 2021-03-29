# Registering a Domain

Route 53 is AWS's DNS service.

It allows you to register doamins, so it can bill you and get a domain added \
to a generic TLD (Top-Level Domain), or a country code TLD registry. \
(TLD examples: .com .net .edu .org .uk)
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

Route 53 → Domains → Pending Requests

Notice the status is "Domain registration in progress". \
We are waiting for this entry to to finish registering and be added to the .org zone file with the .org registry TLD, which is PIR. \
You will also be recieving a few emails, which is expected.

Route 53 → Domains → Registered Domains \
Once registered, click on the Domain record example.org \
This is the info that PIR (.org domain regisrtry) has been given. \
DNS system uses this to point to and resolve anything in our domain.

Route 53 can register domains, and also provide Name Server services! \
These are the Name Servers which have been allocated and automatically added to the example.org entry in the .org Zone File by AWS. \
AWS has also created an object called the Hosted Zone, which is a Zone File for the Domain that we registered. /
That Zone File has been placed on Name Servers that AWS manage.

You can register a domain with Route 53, and then use that interface to point at some name servers outside of Route 53, \
or you can register a domain elsewhere and then create a hosted zone in Route 53, and point that external domain at the name servers that Route 53 gives you.

In this case, we have both in Route 53, so we can move to the Hosted Zones by clicking Manage DNS (button), \
or Route 53 → Hosted Zones \
then click example.org to view the GUI representation of the DNS Zone File.
