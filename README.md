# Tusky Frequently Asked Questions

## Installing Tusky

### What Tusky release should I use?

There are three different releases of Tusky.

- The mainstream release. Unless you've been told otherwise, this is what you want
- Beta releases. These are released to testers before every mainstream release
- Test releases. These are released every time there is a change to Tusky

### Where can I get Tusky?

You can install Tusky from Google Play or from F-Droid.

To do that:

- Install [Tusky from Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)
- Install [Tusky from F-Droid](https://f-droid.org/packages/com.keylesspalace.tusky/)

Before a new stable release, we publish one or more beta releases. If you want to become a beta tester and help us find bugs before they get released to everyone, you can:

- Opt-in to [Tusky Beta on Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)
- Opt-in to receive unstable releases in F-Droid (Settings -> Expert Mode -> Unstable updates) and you will automatically receive Tusky beta versions if you have it installed via F-Droid.

Test releases that always contain our newest code are also available on Google Play and F-Droid:

- Install [Tusky Nightly from Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky.test)
- In the F-Droid settings, select "My Apps > Repositories", and add a new repository with the link `https://releases.nailyk.fr/repo/`

### Why is the Tusky release on F-Droid out of date?

F-Droid builds Tusky from the source code when a new release is made available. This can take longer than it takes for the new release to available on Google Play.

## Managing my account

### Can I create an account with Tusky?

Not yet, you must create an account via a service like https://joinmastodon.org/ first.

Once you have done this you can then log in to the account in Tusky.

### Can I remove my account with Tusky?

You can sign out of your account with Tusky. But you will need to follow your instance's procedure to fully delete your account.

### I'm trying to log in to my account, and am being rick-rolled. Why?

Tusky does not support usage by accounts on some [servers](https://github.com/tuskyapp/Tusky/blob/develop/app/src/main/res/values/donottranslate.xml#L160) because of their association with hate groups.

> A server not being on this list does *not* imply endorsement by the Tusky developers.

If this offends you you are free to use another Mastodon client.

## Timelines

### Why is the count of likes and boosts different to the web?

This is because of how Mastodon works. Likes and boosts do not federate perfectly; if you and the other user are on different servers you will see different numbers between Tusky and the website.

### How do I see the Federated timeline?

From your home timeline:

- Open "Account Preferences" (swipe from the left edge, or tap your profile picture to see the option)
- Tap "Tabs"
- Tap the "+" button (bottom right)
- Choose "Federated" from the menu

You can adjust the order of tabs on this screen too.

### How do I hide boosted posts from my timeline?

- Open "Preferences" (swipe from the left edge, or tap your profile picture to see the option)
- Tap the "Filters > Tabs" section
- Unselect the "Boosts" option

### How do I hide replies to posts from my timeline?

- Open "Preferences" (swipe from the left edge, or tap your profile picture to see the option)
- Tap the "Filters > Tabs" section
- Unselect the "Replies" option

### How do I follow a hashtag?

- Tap the hashtag in a post to view all posts with this hashtag
- Tap the "follow" icon at the top right

### How do I mute a hashtag?

> This feature is available in Tusky 21 or above (including Nightly). To check the Tusky version you are using open the "About" menu.

- Tap the hashtag in a post to view all posts with this hashtag
- Tap the "mute" icon at the top right

## Posting

### How do I edit a post?

> This feature is available in Tusky 21 or above (including Nightly). To check the Tusky version you are using open the "About" menu.

Find the post you want to edit, then:

- Tap the "..." menu at the bottom-right of the post
- Choose "Edit"
- Tap "Toot" to send the edited post (replacing the original)

### How do I send a direct message?

> Important: Direct messages on Mastodon are not encrypted, and can be read by the admins of your instance. Be careful sharing any private information on Mastodon.

- Create a new post
- @-mention the user you want to send it to
- Tap the "visibilty" icon (by default this looks like a globe)
- Set the post's visibility to "Direct"

## Notifications

### Why are notifications less frequent with Tusky?

By default, Tusky checks for new notifications approximately every 15 minutes.

Tusky can also use [UnifiedPush](https://unifiedpush.org/) to show notifications in real-time. To do this:

- Install "ntfy" (from [Google Play](https://play.google.com/store/apps/details?id=io.heckel.ntfy) or [F-Droid](https://f-droid.org/packages/io.heckel.ntfy))

### Why does Tusky use UnifiedPush instead of Google services for notifications?

Google Services don't work on all devices and we want to give users the freedom to chose their push provider.

## Filters

### Will my filters import from my instance?

Yes. Filters will sync in both directions between Tusky and your instance.

## Reporting bugs and making feature requests

### How do I report a bug?

If you think you've seen a bug in Tusky the ideal way to report it is to:

> You will need a Github account to do this.

1. Check that no one else has already reported the bug
	1. Open the [list of open issues](https://github.com/tuskyapp/Tusky/issues)
	1. Search the list of issues
	1. If you find an existing bug report you can leave a comment (if you have extra information to report), or click the "Subscribe" button to be notified when there are other comments on the bug, or when it is closed.
1. If there are no matching reports then click the "New issue" button to report a new bug.
	1. You will automatically be notified when there are comments on the bug report, or when it is closed.

The less ideal way to report a bug is to post about it on Mastodon and either mention the Tusky account (`@Tusky@mastodon.social`), or use the `#Tusky` hashtag, and hope that someone sees it.

### How do I make a feature request?

If there is a feature you would like to see added to Tusky the ideal way to report it is to:

> You will need a Github account to do this.

1. Check that no one else has already requested a similar feature
	1. Open the [list of open issues](https://github.com/tuskyapp/Tusky/issues)
	1. Search the list of issues
	1. If you find an existing feature request you can leave a comment (if you have extra suggestions or more information), or click the "Subscribe" button to be notified when there are other comments on the requests, or when it is closed.
1. If there are no matching requests then click the "New issue" button to suggest the feature.
	1. You will automatically be notified when there are comments on the feature request, or when it is closed.

The less ideal way to request a feature is to post about it on Mastodon and either mention the Tusky account (`@Tusky@mastodon.social`), or use the `#Tusky` hashtag, and hope that someone sees it.

## Contributing to Tusky

### I want to help out, what can I do?

There are many ways you can help Tusky development.

- Bug reports and feature requests
- Translations
- Code and documentation contributions
- Donations

Well-written bug reports and feature requests help make Tusky better for everyone. The previous sections explains how to report bugs and make feature requests.

If you would like to see Tusky translated in to a language that you speak, or you see a problem with one of the existing translations you can contribute by sending in a fix. We use Weblate to manage translations; you can sign up at the [Tusky Weblate instance](https://weblate.tusky.app/) and submit a new translation, or improve an existing one there.

If you are familiar with Android development you can also send code changes via Github. A great way to start is to search the list of issues for a bug or feature request that is important to you, and start discussing how you want to solve it there. After any discussion you can then write the code and submit a PR with the change.

Financial donations are always welcome, and can be done through the [Tusky open collective project](https://opencollective.com/tusky). There you can sign up and make a one-off or recurring donation to the project.

## How can I contact the developers?

In the [#Tusky](https://matrix.to/#/#Tusky:matrix.org) Matrix channel.

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0ODQ3NTQ1NSwtMzUwODUwNTM5LC0yMT
A3OTM0MTgsLTc1MjI0NTIwMywtMTgyNzMyMjcyOV19
-->
