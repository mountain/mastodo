Important Notes Regarding this fork
===================================

This is Mastodo, a Mastodon's fork implementing useful features that will not be implemented upstream. ( Take a look at the different topics on https://discourse.joinmastodon.org if you want to
understand more, but you've been warned, it can be toxic ).
It is deployed on https://mastodon.host, and tends to integrate all the upstream commits ( deactivating stuff that does not make sense of course ).

Patches implemented:
- PIWIK integration ( allows to have some nice anonymous, self hosted and opensource analytics on the visitors ).
- Full Text search for statuses ( upstream code only allow searching users and hashtags, or needs Elastic Search to allow searching your own statuses only ).
- FTS for your home timeline ( not only your own toots, but also people you follow, WIP ).
- 20 results instead of 5 per type of search.
- The FAQ link on the homepage points to /about/more instead of the github repo.
- 1024 character limit for posts instead of 500 ( TODO: implement that as a configuration instead of being hardcoded ).
- 512 character limit instead of 160 for profile bio ( TODO: implement that as a configuration instead of being hardcoded ).
- replies and reboosts are displayed in the timelines instead of being ignored.
- CI to check every user facing function is behaving correctly.
- A few other minor tweaks like full column display to fill bigger screen, multiples themes, and other improvements...
- Oauth patch to allow authentication by either the local username or the email ( necessary for the XMPP integration ).
- Glitch-soc's Vanhj edition is in the glitch-vanhj branch.

Policy on this fork:
- We want to provide a customisable mastodon instance for the admins, allowing them to choose the feature set they want, and a full featured instance for your users. 
- Pull Request welcomed and accepted, whatever your rationale ( if you code something though just for you, or a niche feature, please make it optional and we'll merge it ! )
- We won't reject a feature or a modification because 'I dont like it', ever.

Notes for admins that want to just integrate the patch for FTS ( to allow not using ES and save a bit of resources ): Check the unmaintained FTS_NOES.md file !

Original README is below:

Mastodon
=======
![Mastodon](https://i.imgur.com/NhZc40l.png)


