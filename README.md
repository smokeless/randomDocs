# randomDocs
just random info
Notorious b.s.d. posted:
The problem with Ubuntu isn't a matter of taste. It's not that I don't like Unity, or I have bad feelings about Shuttleworth, or that the logo doesn't agree with me. It's much more fundamental: The Ubuntu model for development is broken.

Ubuntu periodically forks Debian's "Unstable" tree (Debian's rolling release). Canonical, inc. works from that snapshot for six months, and then publishes a Ubuntu release.

Inside that Ubuntu release, there is a core of Canonical-supported packages. Canonical accepts bug reports for these packages. These packages receive updates for the supported lifetime of the release. Ubuntu's "core" is supported much the way that Debian or CentOS is.

The problem is that this core is only a fraction of the packages on the system. Ubuntu 14.04, the latest "long term support" release, contains 44378 packages. Only 8751 of them are in the supported part. The rest of the packages go into a separate repository, "Universe."

The packages in Universe, the missing 35 thousand packages, are six months old on release day. They've gone six months without updates or security patches. By the end of the release cycle, they're five and a half years out of date.

--

Shadowhawk will doubtlessly point out that a legion of unpaid, untrained, unorganized volunteers can "maintain" packages in universe. But it's completely optional. Any given package might be untouched (bad), get backported security updates (good), be updated religiously from upstream (really bad), or replaced with something completely different from debian (really, really bad).

There's no release management process. There are no guarantees about what you find in Universe. It's totally up to the kindness of individual strangers. 

Universe and Launchpad.net are sources of "works on my machine" issues and security holes. And that is all I have to say about that.

-- 

Of course, all this peril can be avoided if you don't enable the "Universe" repositories. If you restrict yourself to the core and update repos, you should have no problems. In that case, Ubuntu could be just fine.

Now let's try to use it.

I'd like to build a ruby application. 
Whoops. There's no bundler. That was part of Universe.

Python? 
Oops. No pypi and no virtualenv. Those are also stuck in Universe.

Java? 
Sorry. Maven was also part of Universe.

Perl? 
Nope, no mod_perl2.

PHP? 
Actually, PHP works fine with only core. All the necessary bits are supported. I can say without any trace of sarcasm that Ubuntu is 100% totally suitable to hosting PHP applications.
