## Types of Kata pages

  - Learning Resources  
    [Resource page](#Resource_page.md) : Kata resource pages are
    used to share any kind of document, web page, video, [Sushi
    Card](Sushi_Card.md), or any other kind of educational
    resource.  
    [Project page](#Project_page.md) : Kata project pages are
    used to share inspiration for projects that can be done with the
    knowledge gained from completing material on resource pages.  
    [Path page](#Path_page.md): Kata path pages tie the whole
    thing together: Resources and projects are surfaced on appropriate
    paths so as Dojo Mentors and Champions can choose a path of
    resources to use in their Dojo.

## Creating Kata pages

These guidelines explain how to create the different kinds of pages on
Kata. In order to create or edit a page you need to be an [approved
editor](Approved_Editor.md). Once you are, just search for a
page name that doesn't exist and you'll be given the option to create
it.

### General knowledge

#### Formatting

Kata is a MediaWiki based site. Please see the [MediaWiki Formatting
help page](https://www.mediawiki.org/wiki/Help:Formatting) for a guide
to the tags and syntax used.

#### Uploading files

If you need to use images, PDFs, or any other kind of file as part of
your resource, you can upload it to Kata by clicking this button.
[Upload your content\! ](Special:Upload.md)

#### Displaying PDFs on a page

Once uploaded, if your file is a PDF you can display it on the resource
page by placing its name into \<pdf\> tags like so:

    [MyFirstWebsite.pdf](../files/MyFirstWebsite.pdf)

#### Displaying image files on a page

Many image files can be displayed on the page simply by using the File
wiki code:

    [[File:HTML_CSS_Beginner_Badge.png]]

Full details on the options for the inclusion of images can be found in
the [MediaWiki help](https://www.mediawiki.org/wiki/Help:Images). If a
particular file format won't display, please contact  for assistance.

### Resource page

#### Example

[My First Website Sushi Cards](My_First_Website.md) — view the
wiki code of the page to see how it's put together.

#### Goals

A resource page should contain a single resource, or set of related
resources, that cover a certain skill level (beginner, intermediate or
advanced). For example, the [My First Website Sushi
Cards](My_First_Website.md) are a single resource, but the
Intermediate HTML cards are a separate resource.

#### Naming resource pages

The page should be named in a descriptive fashion, but avoid things like
arbitrary/incremental numbers or the name of the Dojo or person who
originally created the resource. There is a field in the template to
give credit, but the title should help another Mentor trying to
understand what a resource is.

#### Resource page template

A template is used to create a resource page. If you copy-paste this
sample template into a page and modify the fields indicated in the
comments, you'll get a resource page with the appropriate categories,
search indicies, etc. 

#### Adding a resource to a path

Adding a resource to a path is a simple matter of including a few lines
at the end of the page. You can add the same resource to any number of
paths. It can be a core resource on one path and a supplementary
resource on another. This is the wiki code you need to include: 

### Project page

#### Example

[Python Blackjack](Python_Blackjack.md)

#### Goals

A project page should contain a single project, designed such that it
can be completed when someone has learned everything laid out in the
core resources of a given path up to the level of the project. However,
it is acceptable to also point to supplementary path resources as
required/recommended prerequisites for a project in the event that the
core isn't enough for what's being attempted.

#### Naming project pages

The page should be named in a descriptive fashion, but avoid things like
arbitrary/incremental numbers or the name of the Dojo or person who
originally created the project. There is a field in the template to give
credit, but the title should help another Mentor trying to understand
what a project is.

#### Project page template

#### Adding a project to a path

Adding a project to a path is a simple matter of including a few lines
at the end of the page. You can add the same project to any number of
paths. This is the wiki code you need to include: 

### Path page

#### Example

[HTML Path](HTML_Path.md)

#### Details

Path pages are mostly automatically generated from resources and
projects included via the [InPath
template](#Adding_a_resource_to_a_path.md). All that is required
on the path page itself is a short summary, a list of prerequisite paths
(or the NoPrerequisites template) and, optionally, the badges that might
be awarded over the course of the path. Here is the source for the
[JavaScript Path](JavaScript_Path.md):

    {{Path
    <!-- THE AREA THE PATH ADDRESSES: Programming / Hardware / Design / Other -->
    |area=Programming
    <!-- IF A PROGRAMMING RESOURCE, THE LANGUAGE THE RESOURCE PRIMARILY ADDRESSES E.G. HTML -->
    |language=JavaScript
    <!-- UPDATE WITH THE NAME OF THE AUTHOR, IF KNOWN -->
    |author=[[CoderDojo Foundation]]
    }}
    
    Learn to add interactivity to a website.
    
    ==Prerequisites==
    {{Prerequisite|HTML Path}}
    ==Possible Badges==
    These are the [[badges]] it might make sense to award to Ninjas who complete the appropriate components of this path. <br />
    {{Badge|language=javascript|level=beginner}}
    {{Badge|language=javascript|level=intermediate}}
    {{Badge|language=javascript|level=advanced}}
    {{PathDetails}}

Things to note:

#### Path summary

A short summary of the path is included between the **onlyinclude**
tags, so it can be used elsewhere in the site to summarise the path in
lists, tables, etc.

#### Prerequisites

If there is anything that someone attempting this path should know
first, point to the path(s) that would give them that knowledge. Use the
Prerequisite template to do so as show, as this ties the path into other
paths so as mentors can navigate from one to another as their Dojo
completes them.

#### Badges

Where available, images of the [Zen](Zen.md)
[Badges](Badges.md) have been put on the wiki, accessible
through the Badge template, once passed a language and level, as shown.

#### Path Details

This template automatically finds (and keeps updated) the list of all
core, supplemental and project resources that are tagged for the path,
as well as any paths that list this one as a prerequisite, so as Mentors
can determine where to go next.
