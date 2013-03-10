# GitHub Pages and You

* What is GitHub Pages?
  * Free static site hosting
  * Fully contained within git repository and integrated with GitHub
  * Perfect for documentation and microsites
* How does it work?
  * Special Branches
  	* `gh-pages` for most pages
  	* `master` for `[username].github.com` repos
  * All files transparently published by default
  * Certain files treated differently (more to come)
* Getting Started
  1. Create a new repository in your account, for now, let's call it `simple-site`
  2. Follow the instructions to clone that repository to your computer
  3. `cd` to the directory containing the repository
* Creating your first page
  1. Create an index file (e.g., `touch index.html`) and add a few words (perhaps "Hello world"?)
  2. Add the file to git (`git add index.html`)
  3. Commit the staged changes (`git commit -m 'initial commit'`)
  4. Push the changes back up to GitHub (`git push -u origin gh-pages`)
* Take a look
  1. Navigate to http://[you-user-name].github.com/simple-site
  2. You should now see the contents of your index.html file
  3. *Note: Even for private repos, pages sites are public*
* Adding some formatting
  * The index file is just an HTML file, so there's no reason we can't add some HTML and formatting
  * Take a moment to add `<html>`, `<head>`, and `<body>`, tags to the index file, and any formatting you want
  * Add, commit and push, just like last time (`git add index.html`, `git commit`, `git push`)
  * The changes should now be visible in your browser
* Introducing Jekyll
  * In addition to static file hosting, every push to the `gh-pages` branch is transparently run through the [Jekyll](#) templating engine
  * Jekyll allows you to organize pages by common, reused layouts, and helps to build more complex sites
  * To disable Jekyll, simply commit a file called `.nojekyll` to the repository
* Jekyll Basics
  