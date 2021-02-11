# Contribution Policies

This file is intended to clarify most of the file structure and dependencies in the repo files to produce a super awesome website. The most important rules of contribution are:

1. Always commit *major, and only major,* changes to the files.
1. Use branches if you are going to produce major changes.
1. Never commit without a descriptive message.
1. Don't be afraid to discuss problems using the issues page on GitHub.

The repo is divided onto the following categories:

1. Config file.
1. Gemfiles.
1. Format files.
1. Content Files.
1. Building Files.
1. Image files.
1. Community files.

## Config File

This file is the one in which global variables for automated site generation are defined. The point is that this constitutes a namespace of *place holders* on styling and building files. You may define a global variable for the website here, but please document carefully what the variable represents, and where is it expected to be used.

## Gemfiles

These files tell Jekyll which tools to use to build the website. Modification of them is only advised if you intend to customize Jekyll styling. In that case, you must create a separate branch to commit changes, and merge once they are well tested.

## Format Files

These must be located inside a ```include``` folder. They contain templates for the construction of headers, footers, and other elements of the website. Modification is only advised if a customization of the style is intended. As always, changes are to be performed on a separate branch, and then merged to main.

## Content files

These corresponds to *pages* and *posts*.

### Pages

The website is expected to consist of at least 4 pages:

* Home Page (```index.markdown```)
* Crash Course page (```pages/CrashCourse.markdown```)
* Projects page (```pages/Projects.markdown```)
* About Page (```pages/about.markdown```)

All pages, except *Home Page*, must be stored inside ```pages``` folder. You may not create pages carelessly, for they are linked at the main menu of the website. Always think if it corresponds to either a Crash Course publication or a Project publication before creating a new page. At this early stage, the current contributors do not know how to create subpages or nested menus with Jekyll. Therefore, try to fit publications onto Crash Course, Project or About pages.

**NOTE:** There is a ```404.html``` file that contains the default page when the server is unable to find the content on the repo. This can be personalized, but is scarcely necessary.

### Posts

This are simple blog posts. They are to be stored on the folder ```_posts```. The main rule for posting is to include the date YY-MM-DD in the name of the file, since this is a requirement of Jekyll. Any post must be categorized as Crash Course or Project, and identified as such.

## Building Files

These are html files on ```_site``` folder. They **should not be modified**. These files are generated automatically by Jekyll, and thus their integrity is crucial for the site working correctly. All images are expected to be stored in a common folder ```images``` at the root. They should be given a descriptive name. The only accepted format of images is PNG.

## Community files

These are guidelines for contribution, use of content and description of the repo. The files:

* ```CODE_OF_CONDUCT.md```
* ```LICENSE```

Should be read carefully, but no modified. The files

* ```README.md```
* ```CONTRIBUTING```

May be modified according to the evolution of the website.

---

Thanks for contributing to QC-FEM's site. Make sure to understand all the guidelines stated on this document before making a pull request.
