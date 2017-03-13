# Hello, World

In your first assignment you will end up with a web page, no matter how simple, published on the web.

## Objectives

- Get to know your text editor.
- Introduce yourself to working on the command line.
- Publish a web page.

## Requirements

- First, read [this short article](http://blog.froont.com/brief-history-of-web-design-for-designers/) on the history of web design.
- Compose a short essay (just a couple paragraphs at most) that summarizes your thoughts on the web; where's it's been, and where it's going.
- **Note**: You should complete at least the tasks given for _explorer_ mode as listed below before turning in the assignment, as well as before attempting _adventure_ or _epic_ modes.

### Setup

- First, ensure you have the [`app-app` generator](https://github.com/tiy-tpa-fee/app-app) installed. We may have done this in class, you only need to do it once:

  ```sh
  npm install -g app-app
  ```

  Also, set up hub to use `HTTPS` rather than `SSH` for repositories:

  ```sh
  git config --global hub.protocol https
  ```

- Open your Terminal and create and change into the project's directory:

  ```sh
  mkdir -p ~/tiy/week-1/day-1/hello-world
  cd ~/tiy/week-1/day-1/hello-world
  ```

- Run the generator to create a boilerplate project:

  ```sh
  app-app -alpha
  ```

  Answer "Yes" to the questions about GitHub and Yarn.

- Open the project folder in Atom:

  ```sh
  atom .
  ```

  Remember `.` is an alias for the current directory.
- Tab back to your Terminal and start the development server:

  ```sh
  yarn start
  ```

  This should automatically happen, but if it doesn't; navigate to [http://localhost:3000](http://localhost:3000) in your browser. As you make changes to your code, the development server will automatically refresh this page in real-time.

  While the development browser is running, it will control your Terminal, to exit it, press `Control-C`. You can always start it up again with `yarn start`.

- Using the file browser in your editor, open the file `public/index.html` and format your essay with HTML tags and place them into the document (remember all content goes _inside_ the `<body>` tags). Don't worry about the other files in the directory for now, we'll talk about those later, right now, we're mostly concerned with the two files in `public`; `index.html` and `screen.css`.

### Explorer Mode

- Follow all of the setup instructions.
- All of your HTML (and CSS if you do *Adventure Mode*) should be formatted cleanly and consistently. Remember to check the appearance in your browser as well!
- Spend some more time getting to know your terminal and text editor. Try finding some color schemes you like online and installing them.

### Adventure Mode

- Research the `id` and `class` HTML attributes.
- Use valid CSS to style the page (in the neighborhood of a couple dozen CSS declarations).
- Use at least one image somewhere on the page (like the screen shot of your terminal if you do *Epic Mode*, or anything else you see fit).

### Epic Mode

- Create a full layout for your page (heading, navigation, sidebar, footer, etc.).
- Use more complex CSS selectors than we covered in class.

## Turning In

These steps will be followed for almost every assignment going forward. Once you've completed at least _explorer_ mode and you're satisfied with your work, let's get it published. First let's get it up on GitHub.

- First, let's add all our work to git, and ask it to commit it:

  ```sh
  git add .
  git commit -m "My first webpage"
  ```

  Feel free to replace _"My first webpage"_ with a more meaningful message.

- Push our local commits to GitHub:

  ```sh
  git push -u origin master
  ```

  The `-u` option tells git we want to making pushing the `master` branch to `origin` the default, so next time, we can just type `git push`.

- Now that our source code is up on GitHub, let's publish our page to [Surge](https://surge.sh). The command to do this has already been setup for you:

  ```sh
  yarn deploy
  ```

- Turn in the URL to your repository on GitHub in newline. It should look like:

  > `https://github.com/USERNAME/hello-world`

## Additional Resources

- https://developer.mozilla.org/en-US/Learn/HTML/HTML_tags
- http://atozcss.com/start-here/
- http://www.evolutionoftheweb.com
- [Terminal Themes](https://github.com/lysyi3m/osx-terminal-themes)
- [FiraCode Font](https://github.com/tonsky/FiraCode)
- [Jason's Terminal Theme - One Dark - Matches the Atom theme of the same name](https://github.com/nathanbuchar/atom-one-dark-terminal)
- [Mac Basics](https://www.apple.com/support/macbasics/)
- [Mouse versus Command Line](http://lifehacker.com/5633909/who-needs-a-mouse-learn-to-use-the-command-line-for-almost-anything)
