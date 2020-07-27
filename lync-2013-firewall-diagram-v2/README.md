Lync 2013 Firewall Diagram V2
=============================

            

Recently while on a Lync project I was asked by the Network Manager for a better explanation of the firewall rules that needed to be added.  I had sent the usual spreadsheet/table you get from the Planning Tool and in the [Lync 2013 Detailed Design Calculator](http://gallery.technet.microsoft.com/office/Lync-2013-Standard-Edition-324bf0f1) tool by Alessio Giombini and Alberto Nunes.  I also sent him a brief explanation in words of what I was after.  On top of that I also sent him
 an example of the configuration entries for his firewall with the correct ports and IPs.  Both the static NATs and the access lists.  But he wanted more.  He called it a data flow and explained it as a map of what talks to what and how.

So I took to Visio and made a picture which I hope is worth at least a thousand words.  When I sent it to him he said he immediately got it and created the rules I needed.

Firstly, before I attach the diagram I'll explain a couple of things.  All the data is fictitious as far as I know.  I made up the IPs, public, DMZ and internal LAN.  I'm sure someone has the IPs but any similarities are
 unintentional.  

I've used a public range of 217.207.20.111/28, a DMZ range of 172.22.2.0/24 and an internal range of 192.168.2.0/24.  And the domain is 'domain.com'.  And finally, the server names are based on the role they play in the topology.

The topology is a Lync 2013 Standard Edition Pool Pair Collocating all the Roles.  An Edge Pool with a single member, a reverse proxy using IIS ARR and an Office Web Apps server.

Other than that, I'll let the diagram speak for itself.  I hope you find it useful.  The original post is on my Lync blog

here.  It was so pupular I was getting asked to post the Visio source.  So I did.  Enjoy.


Any questions or comments please let me know.


**Minor Update to Version 2.**  Once again, thanks to Lync MVP Fabrizio Volpe for pointing out that I forgot to add TCP Port 4443 for CMS replication to the Edge.


**Previous update to Version 2 - **Thanks to a few of you for pointing out some errors on the networking and persistent routes.  And for some work by my colleague Ryan Osborne for helping me sort it out.  Also realised I had a
 representation of a certificate on the Outside AV Edge role and of course AV is not a required SAN on an Edge Certificate.  Thanks to my friend, Lync MVP Fabrizio Volpe for pointing this out.


**Update: **[Here is a link to my new Skypr for Business version](https://gallery.technet.microsoft.com/Skype-for-Business-Server-22e3c2e1)


Thanks as well for all the feedback and support here, on my blog and in Linkedin.  Thanks for the several 5 star ratings.  And thanks for downloading it.  I'm very happy you've found it useful.


Please keep the suggestions coming for future releases and updates.


        
    
