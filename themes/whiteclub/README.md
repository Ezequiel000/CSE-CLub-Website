# Whiteclub Hugo theme

---
![Inicio página](https://whiteclub.radio.clubs.etsit.upm.es/hugo-theme/1.png)
---
![Seccion actividades](https://whiteclub.radio.clubs.etsit.upm.es/hugo-theme/2.png)

---

Hugo Theme specially developed for communities, HackLabs, clubs, etc.

## Features

* Home page
* Team tab
* About tab
* Activities tab
* Blog
* Automations with Zapier
* Easy to use
* MathJax support

**Whiteclub Hugo Theme has been developed only on Spanish**.

A demo of this theme on action [here](https://radio.clubs.etsit.upm.es/).

## Installation

`$ git clone https://git.radio.clubs.etsit.upm.es/Whiteclub/Whiteclub-Hugo-Theme.git themes/whiteclub`

Or

`$ git submodule add https://git.radio.clubs.etsit.upm.es/Whiteclub/Whiteclub-Hugo-Theme.git themes/whiteclub`

## Usage

### Configuration

From exampleSite, copy all files and folders to the root folder of your Hugo site and change the fields on `config.tml` as you like.

### Create pages

#### How to add a new post to blog

To add a new post to the blog, copy the file on `exampleSite/blog/2019-01-28-Nombre-del-post-del-blog.md` on the folder `content/blog/` of your site, and name it with a descriptive title:

```
2019-01-28-Nombre-del-post-del-blog.md
```

Folders should be like this:

```
├── content
│   ├── blog
│   │   ├── 2019-01-28-Nombre-del-post-del-blog.md
```

Update the file with the information of the post.

If you want to see the post run `snap run hugo server`.

#### How to add a new activity

To add a new activity to your site, copy the file on `exampleSite/content/activities/2018-12-02-Taller-ejemplo.md` on the folder `content/activities/` of your site, and name it with a descriptive title:

```
2018-09-10-Taller-Arduino.md
```

Folders should be like this:

```
├── content
│   ├── activities
│   │   ├── 2018-09-10-Taller-Arduino.md
```

Update the file with the information of the activity.

If you want to see the activity run `snap run hugo server`.

#### How to add new people to Team

Team's tab has the board member's information every year. To add new people to team tab (Example: a new board) copy the file on `exampleSite/team/1819/NOMBRE.md` on the folder `content/team/YEAR` and name it with the name of the person. If you want to sort it (president first), you can put a number first:

```
1FranAcien.md
```

Folder should be like this:
```
├── content
│   ├── team
|   |   ├── 1819
│   │   |    ├── 1FranAcien.md
│   │   |    ├── 2NachoLopez.md
│   │   |    ├── 3SergioSanchez.md
```

Update the file with the information of the person.

Pictures should be stored on `static/team/`, and to reference it will be `/team/facien.jpg`, for example.

#### Automations with Zapier

Zapier is a platform for automate actions. Whiteclub Hugo theme has a RSS with activities, and posts, for automate actions with Zapier. For example, send a mail when there is a new Post on the blog, or tweet a new activity.

Rss links are on:  
  * Activities on `https://YOURSITE/blog/index.xml`
  * Posts on `https://YOURSITE/activities/index.xml`

With Zapier you are able to catch the important information, and *zap* a new action.

#### Math equations

Math equations are done with MathJax, `following LaTeX syntax`.

Math equations will be as:

```
<div>
$$
\sqrt{\frac{\lambda}{\ro}}
$$
</div>
```

There is a problem with Hugo rendering `_`, that is used on MathJax. So, you have to put like `$ 2\_{asdf} $` or `$ var_ 2$`.
