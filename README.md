## This is a WIP FAQ for Tusky | Frequently asked questions about the Tusky Mastodon client

Which will include some experimentation with tools to write this FAQ and sync it with GitHub, by @mal0ki (current tool is StackEdit).

## FAQ
**Question:** When will the latest version of Tusky be available on F-Droid?

**Answer:** F-Droid works differently than Google Play. We as the developers do not upload anything, F-Droid builds the app from source once we tag a release in our code repository. This is super awesome because you are guaranteed to get the exact code from our repo, but also means it takes longer for releases to be available.

##
**Q:** Why didn't Tusky support push notifications?

**A:** Pushing to devices would require us to use proprietary Google libraries and to run a relay server. Since we want Tusky to be pure FOSS (free and open-source software) and don't want to send any data to Google we decided not to implement push notifications previously. We have now found a solution that works for us without compromising our principles.
##

**Q:** Will my filters import from my instance?

**A:** Yes. Filters will sync in both directions between Tusky and your instance.
##

**Q:** I want to help out, what can I do?

**A:** You can help translating Tusky into your language on our [Weblate instance](https://weblate.tusky.app/) and report bugs or even send us fixes on the [main GitHub repo](https://github.com/tuskyapp/Tusky). If you plan to contribute bigger changes, please contact us first.
And don't forget to tell your friends about Tusky! You can also donate to us through Open Collective.
##

 **Q:** Can I try out the beta? 

 **A:** You can sign up for the [Google Play beta, via this link](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)
##

**Q:** What about Nightly releases?

**A:** The Tusky nightly is [available on Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky.test) as well. On F-Droid, [add this repo](https://releases.nailyk.fr/repo/).
##

**Q:** The likes and boosts aren't displaying the same numbers as on the web?

**A:** This is not a Tusky bug, it's because boosts and likes do not federate perfectly. I.e., if you and the user whom you see this on, are not on the same server you will see different numbers on Tusky and on their message on the web.
##

**Q:** How do I remove an account from Tusky?

**A:** Just select the account, then log out.
##

**Q:** My instance has a custom character limit, but Tusky allows only 500 characters

**A:** Your instance needs to make this information public via the `max_toot_chars` property of the `/api/v1/instance` endpoint. Contact your admin to change this. See e.g. here https://pleroma.site/api/v1/instance for a config that works with Tusky.
##

**Q:** Will you block more domains than the Gab related ones?

**A:** The size of Gab is pretty unique and we have no time to research smaller instances, so most likely no, but it's always a possibility.
##

**Q:** Is this censorship/against free speech etc.? 

**A:** No because of three reasons, 1, hate against marginalised groups is not an opinion; 2, Gab can still be accessed by other means and Tusky can be forked; 3, Tusky is no government, so it cannot take away your basic rights.
##

**Q:**
**A:**
##

Template:
**Q:**
**A:**
##

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0ODQ3NTQ1NSwtMzUwODUwNTM5LC0yMT
A3OTM0MTgsLTc1MjI0NTIwMywtMTgyNzMyMjcyOV19
-->
