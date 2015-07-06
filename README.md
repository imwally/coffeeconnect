# starbucksconnect

A shell script that will connect (authenticate) to Starbucks WiFi without the
need of a browser.

## Requirements

* curl

## Why?

Connecting to the wireless network at Starbucks requires you to open a web
browser and click the big green "Accept & Connect" button.  The problem is that
if you're running a web browser with privacy minded add-ons such as Firefox
with [HTTPS Everywhere](https://www.eff.org/https-everywhere) then chances are
you'll be greeted with an HTTPS error page. Of course you could disable HTTPS
Everywhere, try again, click the green button, and then re-enable the add-on.
But that's too much work. And what if you forget to re-enable HTTPS Everywhere?
Not cool dude.

## MAC address parameter

You may also notice the script does not POST your MAC address to the submit
page. To my surprise it's not a required parameter. Regardless if this adds any
layer of anonymity it should be noted that any network you connect to will
record your MAC address. It's best to spoof your address BEFORE you even
enable your network interface and send any packets to the access point.
