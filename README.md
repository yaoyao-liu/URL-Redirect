# URL Redirect via GitHub
Sometimes, you register a domain but you don't have a server. You may want this domain to redirect to your homepage/FB/IG or etc. However, most domain registrars do not provide this service, or this service charges. At this point, you can do URL redirecting with the github page.

First, create a new empty repo and import this repo to it.

Second, configure a `CNAME` record to your domain as follows:
```
Host: whatever you want. e.g. "www" or "@"
Target / Canonical name: your_username.github.io.
TTL: 10 min
```
You may also configure an `A` record instead of the `CNAME` record as follows:
```
Host: whatever you want. e.g. "www" or "@"
IP: 185.199.108.153
    185.199.109.153
    185.199.110.153
    185.199.111.153
TTL: 10 min
```

Third, change the contents of the [CNAME](./CNAME) file in the repo to your domain.

Fourth, replace the URL is the [index.html](./index.html) to whatever your want.

There is also a [Chinese version](https://github.com/y2l/URL-Redirect-zh/) for this repo.
