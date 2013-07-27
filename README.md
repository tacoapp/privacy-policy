# Privacy Policy

## How We Think

First and foremost, we use Taco ourselves. As users, we want:

* [Easy data removal](#easy-data-removal)
* [Conservative defaults](#conservative-defaults)
* [Fanatical security](#fanatical-security)
* [Real transparency](#real-transparency)
* [No finger pointing](#no-finger-pointing)
* [Auditable humans](#auditable-humans)


## Easy Data Removal

We only want to store what you want us to. At any time, you can revoke
some or all of Taco's permissions or close your account entirely. Doing
so is self-service via the Taco Web site (we hate that "Email us to
close your account" gimmick as much as anyone). All online data for your
account is deleted immediately and any backup copies will be deleted
within 7 days.

## Conservative Defaults

How many times have you logged into a service for the first time in
months and discovered long-forgotten data? If you aren't actively using
Taco, we don't need your private data. After 3 months of inactivity,
Taco will automatically delete your connector service credentials and
Taco's copy of your tasks (without affecting tasks on the linked
service).

Taco is one of very few services with such a "[Dead man's switch](http://en.wikipedia.org/wiki/Dead_man's_switch)"
and it's because we are users first. A user should be able to safely
walk away and not be surprised when they return 6 months later. When you
want to use Taco again, just re-link the services.

We ask for the least amount of access required to deliver Taco. For
example, our Google Tasks permission request does not give us access to
GMail, Docs, or any services other than Tasks.

We store the least amount of data required to deliver Taco. For example,
a Basecamp API request for a list of tasks will also return information
we don't need, such as the task creator. That information is not
retained. The Taco Web site displays substantially all task-related
information that Taco has.

We proactively look for opportunities to retain less trust. For example,
we sent GitHub a detailed, unsolicited suggestion that they support a
new OAuth [scope](http://developer.github.com/v3/oauth/) with less
access than is currently provided.

If you email us a question, our support inbox may retain your email (and
thus your email address). We will not use your address for any purpose
other than responding to your inquiry.


# Fanatical security

Security is all about reducing risk. We will never knowingly send
passwords, credentials, or tasks without encryption ("cleartext"), nor
make it possible for you or underlying services to do so. To that end,
all of tacoapp.com is delivered over HTTPS (SSL encryption). 

Taco is hosted on [Heroku](http://www.heroku.com/). This has many
benefits, but one of the largest is that Taco runs on a server
architecture that is used by hundreds of thousands of other Web
applications.  Heroku's infrastructure receives a level of testing and
monitoring that would be very difficult to obtain any other way.

Because we store access information for your accounts on other services,
we have a healthy paranoia about data store security. All credentials
for remote services (such as API keys, OAuth tokens, and RSS URLs) are
encrypted when stored by Taco. This means that a database breach alone
would not disclose usable credentials.

Further, Taco encryption keys are a combination of strings stored in the
app (source code), memory, and a database. In order to obtain a key, an
attacker would need access to all three. Finally, credentials are only
decrypted for the time needed to perform an update (typically 3 seconds
or less) and only in memory. While nothing is completely bulletproof,
this is as good as is practical given that Taco needs to use the
credentials, and is far beyond most services.


# Real transparency

If we have a security breach or have reason to suspect one, we will
email you and blog publicly about it. This disclosure will receive the
same amount of publicity as would a positive announcement.

We will keep this privacy policy current as needs change. All changes to
this privacy policy are tracked in a revision-control system
[here](https://github.com/tacoapp/privacy-policy) so anyone can easily
examine all changes.

Modifications to this policy take effect 15 days after the change. While
most privacy policies state that changes take effect immediately, we
always want you comfortable with terms before they happen. And if you
see something that you don't like, please let us know. We probably
either need to change it or make the explanation clearer.

Clearly stating small things matters too. Taco uses cookies to identify
the account you are logged in to, as do almost all password-protected
Web sites.  Those cookies are currently: tacoapp.com, Google Analytics.
We proudly track aggregate usage metrics because it tells us which parts
of Taco should receive more attention. As users, we want the most useful
features to grow.  We do not track individual behavior except as kept in
Web application server logs for
[troubleshooting](http://guides.rubyonrails.org/debugging_rails_applications.html).

We don't hide behind obscurity or lack of specificity. For example, Taco
uses [attr_encryptor](https://github.com/danpal/attr_encryptor) for
encryption and [devise](https://github.com/plataformatec/devise) for
authentication. We are proud to share our infrastructure because we take
pride in it. We'll do our best to answer all good-faith questions about
Taco's operations.


# No finger-pointing

Although we will clearly disclose how Taco uses other services, we are
responsible for your data. You are trusting us. A violation of this
privacy policy means we failed, not some other party.

Regarding services, we use third-party services for email delivery,
performance monitoring, metrics, and other ancillary services, but do
not disclose any service credentials with those third parties. Task
lists are only disclosed to third parties to provide features that you
have requested.  For example, as part of delivering daily task lists,
our email provider sees the email message which contains your active
tasks.

Our hosting service Heroku is the only other entity with any access to
service credentials. We've intentionally chosen them as one of few
services worthy of that trust (and even in that case, to borrow from the
axiom "Trust, but verify," we trust, but encrypt).

We will never disclose your personal information to other entities
except: to deliver the service as described above; in the event of an
acquisition or transfer of substantially all assets of Taco; or when
required by law.

If an acquisition involves personal information, the acquirer will be
bound by this privacy policy at the time of acquisition (so that
modifications would still require 15 days of notice). If a disclosure is
required by law, we will publish as much as possible without
imprisonment (following Google's transparency [report](http://www.google.com/transparencyreport/).


# Auditable humans

The two principals are the only people who have access to any private
user information. We only use it for troubleshooting, which is usually
at your request.

Taco has no Web-based "admin view" where admins can see your tasks.
Viewing any task data is and should be annoyingly difficult for Taco
principals, not a routine task.

Further, except for operational emergencies, we will always ask for your
explicit permission before any other human sees the text of a task.  In
most cases, task labels are not helpful for troubleshooting.

In the case of operational emergencies (or any other case where a human
sees your task data without your explicit permission), we will notify
you and provide an explanation within 24 hours.

Taco is operated by two people who have [real](http://twitter.com/troyd)
[names](http://twitter.com/fixie) and personalities. We may sit across
from you in a Seattle coffee shop from time to time. There's nothing
faceless about us.

Our commitment to you is that we'll evaluate decisions as users: first,
last, and only.
