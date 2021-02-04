## Y THO
We want all traffic to https://links.territoryfoods.com to be proxied to
https://links.iterable.com.

We could do some cloudfront stuff, or, we could do this. We did this.

The app shouldn't ever really be hit w/the nginx proxy that is setup via
buildpack settings. See that config here:
https://github.com/powersupplyhq/iterable-links-redirector-proxy

If by some happenstance it does get hit, then web.js will be executed.

## Credit
kenmickles/heroku-redirect
