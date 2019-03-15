# Rick's personal site Github

Welcome to the GitHub repository of my personal site! The live site is located at https://www.rickyuan.com/.

It was created from the [Start Bootstrap - Resume](https://startbootstrap.com/template-overviews/resume/), template released under the [MIT](https://github.com/BlackrockDigital/startbootstrap-resume/blob/gh-pages/LICENSE) license.

## How I set it up
At my DNS provider, I setup two records:
1. An `A` record called `rickyuan.com` that points to GitHub's servers:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

2. A `CNAME` record called `www.rickyuan.com` that points to
`ricksyuan.github.io`

To verify that the links are pointing properly, the following two commands should resolve to the same IP address:

```
dig rickyuan.com +noall +answer
dig ricksyuan.github.io +noall +answer
```

### References
https://help.github.com/en/articles/setting-up-an-apex-domain-and-www-subdomain
https://help.github.com/en/articles/setting-up-an-apex-domain

## Usage

Open `index.html` in a web browser

Run `npm install` and then `npx gulp dev` to watch changes