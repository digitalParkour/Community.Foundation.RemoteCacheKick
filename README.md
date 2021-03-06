﻿﻿Sitecore - Remote Cache Kick
==============

Summary
--------------
Adds a button to the publish ribbon so users (with access) can clear the remote server caches.

![alt text](https://github.com/digitalParkour/Community.Foundation.RemoteCacheKick/raw/master/screenshots/Button.png "Custom cache clear button in publish ribbon")

Implementation
--------------
A custom remote event is used to broadcast the button click.
An event handler is used to respond to the remote event and clear server cache.

Special thanks to [Kasaku on sitecore.stackexchange](https://sitecore.stackexchange.com/questions/2271/clearing-cd-cache-in-code-from-the-cm) for outlining the approach.

Installation
--------------
Either:
* Install Sitecore package. [See Releases](https://github.com/digitalParkour/Community.Foundation.RemoteCacheKick/releases).
	> For scaled setup, also copy files (config and dlls from package) to CD servers.

Or:
1. Include this project in your Helix style solution
2. Update NuGet references to match target sitecore version
3. Sync unicorn data or install sitecore package
    > Expects Unicorn 4+ in your solution.
    > If not using Unicorn, disable Foundation.RemoteCacheKick.Serialization.config