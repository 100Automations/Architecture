# Collections

## `_automations/`

100 Automations is a website built to host Automations or automatic software programming.
Those Automations are stored in our collections as data in Ruby.

There is no markdown contained within the file.
If you want to display the data within automations you will have to iterate through the data using liquid.

## `_guides/`

In addition to the front matter inside of a guide there is also markdown content.
This content is displayed accessing the default `content` property.

This file is viewable because our config.yml file states that the output of this file should be viewable.
There is also a layout under the same name that coordinates how each guide should be displayed.

## `_bios/`

If you are on the 100 Automations team, either building an automation or the website, you will be creating a bio.
Bios are like automations, they only contain front matter and contain no content in markdown.

## `_social-media-posts/`

The images for social media posts is also located in the `assets/images/`.
However each document in social media posts is for each social media network.

```yml
---
have-an-idea: 
    src: assets/images/social-media-posts/FB-have-an-idea.png
    alt: Have an Idea?
host-automation: 
    src: assets/images/social-media-posts/FB-host-automation.png
    alt: Host An Automation
logo: 
    src: assets/images/social-media-posts/FB-logo.png
    alt: logo
social: Facebook

---

```

This is the social media posts that we have for Facebook.
The other documents in the collection reference different images for their social media website.

## `_memes/`

The content for Memes is located in the front matter.
The data located in memes is the url of the static `assets/images/`.

There is also an alt and title to describe the picture.
