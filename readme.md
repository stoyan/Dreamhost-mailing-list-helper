# Dreamhost's Announce Lists helper

Dreamhost offers a free mailing list that you can setup. Read about it here: https://help.dreamhost.com/hc/en-us/sections/203272168-Announcement-Lists

So here's what you do:

Download these HTML pages. Customize them. Put them up on your server, e.g. in /mail/ directory. Then complete the setup on the Dreamhost's panel.

Enjoy a free mailing list setup that you fully control and own too!

# The pages to customize

 * `form.html`: subscription form. Just a chunk of code to copy/paste in a larger template
 * `formunsubscribe.html`: sad little page to let people go
 * `invalidurl.html`: The URL of the page that will appear if the email address entered is invalid
 * `alreadyonurl.html`: The URL of the page that appears if someone who is already on the list attempts to subscribe to it
 * `checkyourmailurl.html`: The URL to tell people to check their email
 * `emailconfirmurl.html`: The URL of the "welcome" page that will appear when the user confirms their opt-in to your list by clicking a link in an email message just sent to them
 * `notonurl.html`: The URL of the page that appears if they are not on the list, and they have attempted to unsubscribe
 * `unsuburl.html`: The URL of the "goodbye" page that appears if someone successfully unsubscribed from the list

# Example flows

## Example subscription flow
 
form -> invalidurl -> form -> alreadyonurl -> form -> checkyourmailurl -> (checks mail) -> emailconfirmurl

## Example unsubscription flow

(mail unsubscribe link) -> formunsubscribe -> notonurl -> formunsubscribe -> unsuburl

# Completing the setup form

In Dreamhost's setup form enter these URLs:

 * Subscribe URL: https://www.example.org/mail/checkyourmailurl.html
 * Unsubscribe URL: https://www.example.org/mail/unsuburl.html
 * Already Subscribed URL: https://www.example.org/music/alreadyonurl.html
 * Not Subscribed URL: https://www.example.org/music/notonurl.html
 * Invalid Email Address URL: https://www.example.org/music/invalidurl.html
 * Confirmation URL: https://www.example.org/music/emailconfirmurl.html
 
# Referral

If you don't already have Dreamhost, sign up with my referral link http://www.dreamhost.com/r.cgi?447675