---
title: Building my website
date: 2025-03-06
draft: false
tags:
  - projects
  - webdev
---
## Why did I decide to build a personal website?

Overall, the goal is to share more of about what I have going on than can be found on my [LinkedIn](https://www.linkedin.com/in/clmangham/) because it's *really* just a resume and I *really* don't use the social media aspects of it or any other social media platforms. 

Creating a personal website has been a goal of mine for a while now, and while this is not the first version of an online platform for my content, I think this is a better one. Previously, I used [streamlit](https://streamlit.io/) to build and deploy a personal webpage along with an LLM application. As a python programmer, I found it quite simple and intuitive (in fact I may still continue to use it for other projects). After deploying on the free "Community Cloud" I discovered that after a while with no traffic the whole application shut's down (which is fair).

![Image Description](/images/Pasted%20image%2020250306045600.png)

I wanted a better hosting option with more interesting customization options, more control, and the ultimate goal of hosting the site and related services (such as LLM applications) from my secure local network. In addition, I wanted a blog style website instead of a portfolio / personal brand style website. I primarily take notes and do my writing in markdown, so turning those notes into webpages was high on my list.

## Deploying with Hugo and GitHub Pages

I reviewed a few development frameworks starting with the familiar python [Flask](https://flask.palletsprojects.com/en/stable/), and checked out [Jekyll](https://jekyllrb.com/) (based on Ruby), but realized I need to learn way more about frontend. For now I settled on [Hugo](https://gohugo.io/) (based on Go), which seems to be extremely lightweight, easy to customize with themes, and *natively uses markdown to generate html content*. 
### To set up the site
1. Follow the [Quick start](https://gohugo.io/getting-started/quick-start/) guide installing Hugo and its prerequisite Go. I already had Git and did not need Dart Sass. 
2. Download a custom [theme](https://themes.gohugo.io/).

The quick start guide is well done - after walking through the process you can easily replicate it with your theme of choice, configure the site, and add content.

### To host and deploy
For deployment options for now I'm using [Github Pages](https://pages.github.com/) for automatic deployment and CI/CD. This is relatively simple, free, and allows me to stand the site up now as I flesh out content and prepare for local deployment. To do this I just followed the Hugo documentation on [hosting and deployment](https://gohugo.io/host-and-deploy/).

*One thing that does not seem to be mentioned in the Hugo docs is that the github repository name should be username@gituhub.io, this is explained in the Github Pages docs.*

As I mentioned above, this deployment is temporary as I plan to host a different way in the future.

## Why Move to a Secure Local Server?

Mainly because It's a fun homelab project. Of course there *are* limitations to GitHub Pages as it's mainly used for small static sites. From my understanding there is no backend processing and limited control over infrastructure. Ultimately I'll want to have additional services running such as local LLM-powered tools and may even move to dynamic content in the future. Additionally, I am also focused on security and privacy considerations. More on that to come.

## Future updates
- Setting up *and securing* a local server (looking at you [nginx](https://nginx.org/), [Docker](https://www.docker.com/))
- Hosting and serving my website locally (and implementing HTTPS with [Let's Encrypt](https://letsencrypt.org/))
- Adding advanced features and integrations (LLM tools, analytics, content engagement et cetera)





