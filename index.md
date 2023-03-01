---
layout: default
title: Home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# Theme documentation for @yosileyid's Jekyll themes and plugins
{: .fs-9 }

[Jekyll][Jekyll] is a framework built on Ruby that makes creating static blogging sites really easy. I enjoy creating themes and plugins to make it easier for everyone to get online and have their own site. These docs will hopefully help you to get up and running using Jekyll and possibly even with one of my themes. 
{: .fs-6 .fw-300 }

[Jekyll Newspaper Theme][Jekyll Newspaper Theme]{: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[View GitHub Repo][Jekyll Newspaper repo]{: .btn .fs-5 .mb-4 .mb-md-0 }

---

{: .warning }
> This website documents the features of the current `main` branch of the themes for Jekyll created by @yosileyid See [the CHANGELOG]({% link CHANGELOG.md %}) for a list of releases, new features, and bug fixes.

## About the project

This Documentation is &copy; 2023 by [Yosi Leyid](http://yosileyid.github.io). Links will walk you through setting up jekyll blogs on your local computer, you will need to have `Ruby`, `rvm`, `bundler`, and `jekyll` all installed before you can use these themes. Please visit the [Jekyll][Jekyll] site and make sure to install everything you need before using these docs. You may run into issues otherwise.

### License

Just the Docs is distributed by an [Mozilla Public License v2.0](https://github.com/yosileyid/docs/tree/main/LICENSE).

### Contributing

When contributing to the documentation repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/hasidicdevs/hdg-docs#contributing).

#### Thank you to the contributors of these docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"></a>
  </li>
{% endfor %}
</ul>

### Code of Conduct

I am committed to fostering a welcoming community. I use this Code Of Conduct, I believe it includes everyone.

[View Code of Conduct](https://github.com/yosileyid/docs/tree/main/CODE_OF_CONDUCT.md) on our GitHub repository.

----

[Jekyll]: https://jekyllrb.com
[Jekyll Newspaper Theme]: https://yosileyid.github.io/jekyll-newspaper/
[Jekyll Newspaper repo]: https://github.com/just-the-docs/just-the-docs
[customize]: {% link docs/customization.md %}