# Let's Make A Blog

In this assignment, we will update our GitHub pages websites so that they will be a **bit** more dynamic (and interesting) than before.
We will accomplish this by using [Jekyll](http://jekyllrb.com) to combine **HTML templates** and **data** to generate a static website.
This won't be **trully** dynamic, but it will at least give us a feel for how real web applications separate their **data** and 
**presentation** in order to create more flexible websites.

## This Looks Familiar

Yes, this should look familiar to you, because we wrote this skeleton together in class. If it doesn't look familiar then **pay more 
attention in class** or **start coming to class**. For this assignment, we will be taking this skeleton and using it for your own 
blogs, then you will be adding some features of your own.

**NOTE**: you are free to come up with your own titles and things for your blog, but you **must** create something that meets the 
specified requirements.

> Be aware that sometimes it takes a couple of minutes for GitHub to build your website, so be patient when trying to figure out
> whether or not things are working. If the waiting bothers you, you are also free to install a local copy of Jekyll on your
> machine which you can use to get instant feedback from your changes.

## Directions

### Copy Skeleton

First, you will want to copy the files in this skeleton into your github pages repository (this should be a repository called something like 
*yourusername*.github.io). You should already have an index file there, but don't worry about overwriting it. Your history can always 
be checked to ensure that the old work was there. 

**Note**: You should not *fork* this project. You need to copy the contents into your own repository which you have already created.

#### Changes

The code fro mthe skeleton will not work quite as is. Once you copy the files, remove the first line from the configuration file. 
This was only needed for the demo in class.

#### Confirm Your Work

Once you have taken care of the above, go to your GitHub pages url (again, something like *yourusername*.github.io) and confirm that 
your pages has loaded as expected, that the links work, etc.

### Individualize

Once you have copied the included files and confirmed that your blog is working, individualize the blog with your own blog title, etc. 

#### CSS

**Add a CSS file** and link it to the *main layout* (if you link it in the main layout, then it will be pulled into all pages...like magic).
Use this CSS file to style your web blog. I have no specific requirements, but make it clear that you have at least put some effort into
creating something more interesting than what we started with.

#### Now Page

The about page describes you, in general. A [now page](https://nownownow.com/about) describes what you are focused on and doing at 
*this point in time*. For instance, you may have grown up on a farm, but what's more important is *what you are currently doing with your 
life*? What are you focused on? What are you passionate about now? 

Create a "now page" and add a link to it in the main layout (with the rest of the links).

(Side note: If you can't populate a now page, then maybe you should take some time to think about what you would like to be doing with
your life so that you *can* populate this page. For the purpose of this exercise, you can put whatever you want here, but if you can
discover something that you *want* to do with your CS degree *now*, it makes motivating yourself to learn and advance as a professional
much easier!)

#### Confirm Your Work

Be sure to confirm that all of the work you have done up to this point is working as expected when you visit your public url!

### Projects

We want to have blog posts on our blogs, of course, but it would also be nice to have a portfolio of your projects which you can show off.
Accordingly, you should add a "projects" page and add a link to it in your main layout.

#### "Automate"

Of course, you should not be manually adding project information to the projects. Instead, you should create your projects page so that
it loops through your project data and generates previews for each project. Each preview should have a link to the individual project page,
which should be created in a manner similar to how we creates *posts*.

#### Collections

Jekyll is aware of the concept of *posts* out of the box. However, if we want to introduce some *other* type of pages, we need to define
this in configuration file. For our projects, you will need to add:

```yaml
collections:
  projects:
    output: true
```

Once you have made this change, you can add project pages to the *_projects* folder and render them much like how we handle *posts*.

#### Metadata

We want our previews to be a bit different from our post previews, though. We want to add the following metadata fields to the
"front matter" of each project page:
* course number
* description
* image
* topics

##### Course Number

For each project, add the course number for the course the work is related to (or none if it is a personal project). The format should 
be, e.g., **CSC-425**. 

##### Description

This should provide a short description of your project.

##### Image

This should be the url of a screenshot from your project. Create a directory in your GitHub pages repository called *images* to store
all of these screenshots.

##### Topics

This should be a list of topics that are relevant to your project. For instance, this could include the subject, the tools/languages used,
or anything else that might be relevant.

Note that lists of data must be formatted as:

```yaml
topics:
  - something
  - something-else
  - last-topic
```
##### Template

Once you have this metadata added to your project pages you should alter the template for your *projects* page so that it uses the metadata
when generating a preview for each project page.

#### Confirm Your Work

Again, be sure to confirm that your code is actually working as expected when the blog is visited via its public url.

## Give A Damn

I am not specifying how, exactly, your pages have to look or specifying the exact data you need for every page. I **do**, however, expect
you to actually give a damn about the quality of your work and to actually put forth an effort to make something nice. I am **not** 
expecting elaborate CSS, etc. Your page can be plain, but if every page is one line of text and your style sheet is one or two definitions
you **will not get full credit for your work**. Take some pride in your work and make something worth making!
