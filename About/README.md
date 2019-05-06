---
title: About
has_children: false
---

## GitHub Pages
**GitHub Pages** is a static site hosting service designed to host your personal, organization, or project pages directly from a GitHub repository. If the site is a User Page, than it has a repository named **[username].github.io**. If the site repository doesn't have a `master` or `gh-pages` branch, the GitHub Pages publishing source is set to `None` and the site is not published.

### Quick run
* For Repository Name, enter _[username].github.io_
* Make the repository **Public**
* Check **Initialize this repository with a README**
* Click _Create Repository_

## GIT Playbook
The project documentation uses [GIT Playbook](https://github.com/thomasreinecke/git-playbook) project hosted on GitHub. The playbook page comes in a pretty slick but still very powerful look & feel. The main components are:
* **Configurable Title**: What ever you want it to be called, you can easily configure that
* **Live Search**: The content is fully indexed and users can utilise this component to filter based on keywords and based on Topics (topic:myTopic to find all documents that carry this topic)
* **On or multiple Major Sections**: When you actually need more than just one Playbook you can add them here OR you can reference one of the pages you will create and expose that on this prominent spot on the header
* **Table of Content Views**: Documents that have no content but only Child docs show up as ToC pages that hold a number of Tiles. You can use these Tiles to dive deeper into the documentation
* **Tiles with Title, Icon & Description**: Sitting on a ToC page a Tile can be an actual document or a nested ToC page. A Tile comes with a Title, a very brief description and a free Icon from the Font Awesome 5 library
* **Table of Content for the Major Section**: This is a component thats rendering a nice ToC for the full hierarchy of content that was configured for the Playbook

### Steps
1. Fork [GIT Playbook](https://github.com/thomasreinecke/git-playbook) repository
2. Edit _"src/pageConfig.json"_ and change the document structure as you desire
3. Write your documents in Markdown and put them into the _"static"_ folder
4. Create a GIT repository and import your playbook trunk
5. Deploy it with `npm run gh-pages`
6. In GitHub repository > Settings > scroll down to "Github Pages", make sure it points to your "gh-pages" branch
7. Find the link to your GithHub page deployment on that screen aswell: _https://[username].github.io/[repository]/_

### Quick run
1. Fork Fork [GIT Playbook](https://github.com/thomasreinecke/git-playbook) repository
2. Change Repository name
3. In GitHub repository > Settings > Change Source to **master branch**
4. In GitHub repository > Settings > Change Source to **gh-pages branch**
5. In GitHub repository > Settings > Change Source to **master branch**
6. Find the link to your GithHub page deployment on that screen aswell: _https://[username].github.io/[repository]/_