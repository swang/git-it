# Contributing

The app and the guide —

## The App

- Git-it is a terminal app built in the [nodeschoo.io](http://www.nodeschool.io) style with a branch on my [fork](https://github.com/jlord/workshopper/tree/verify) of the [workshopper module](https://github.com/rvagg/workshopper). I've forked it to make changes due to the fact that unlike the other workshopper apps, users aren't creating code to be tested. They are, instead, doing things with Git which can be verified through Git.

- For the most part, challenges are verified using Git itself and comparing the output to the expected output.

- The verifiying of some challenges (that require the GitHub API) and the similated collaborator parts of Git-it are done via @reporobot, who lives on a server running this code: [jlord/reporobot](http://www.github.com/jlord/reporobot).

- The some of the challenges require users to work with a repository that they fork and pull request against. That repository is [jlord/patchwork](http://www.github.com/jlord/patchwork) (named after [teaching night](https://github.com/blog/1747-introducing-patchwork) I host at GitHub HQ with Git-it.).

- The [jlord/patchwork](http://www.github.com/jlord/patchwork) is a site hosted through [GitHub Pages](pages.github.com) that is rebuilt by @reporobot each time a new user completes the challenges with their pull request merged. The site: [jlord.github.io/patchwork](http://jlord.github.io/patchwork)

- The [jlord/patchwork](http://jlord.github.io/patchwork) repo has backups of the template and contributors.json, but what actually matters are the versions on the server with @reporobot, so changes to that should be made on [jlord/reporobot](https://www.github.com/jlord/reporobot)

### To Install

```bash
npm install -g git-it
git-it
```

### To Run from Source

```bash
git clone https://github.com/jlord/git-it.git
cd git-it
npm link
```

## The Guide

- The guide is a static site within /guide in the repository.
- Edits to the text for challenges should be made to the files within `/raw-content`, as those are turned into `/challenges` by the build script.
- Build the site by running `npm run build` from within `/git-it`
