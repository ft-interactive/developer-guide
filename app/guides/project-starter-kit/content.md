## Scaffolding a new project

### The quick way (Mac-only for now)

Make sure you're in an empty directory, then run the quickstart script:

```sh
$ curl -L https://raw.githubusercontent.com/ft-interactive/psk-quickstart/master/quickstart.bundled.js | node
```

You now have a new project based on the starter kit.

### The slow way (any platform)

Just do what the [quickstart script](https://github.com/ft-interactive/psk-quickstart/blob/master/quickstart.js) does, which is:

1. [Download a zip](https://github.com/ft-interactive/project-starter-kit/archive/master.zip) of the Project Starter Kit.

2. Extract the zip. You should have a folder containing a bunch of files (such as <kbd>gulpfile.babel.js</kbd>). Rename the folder to something appropriate for your project.

3. Delete stuff you don't need: the <kbd>docs</kbd> folder and the <kbd>README.md</kbd>.

4. Initialize it as a git repo (<kbd>git init</kbd>, or use SourceTree or something) and do an initial commit of all the files in the starter kit (e.g. <kbd>git add .</kbd> and <kbd>git commit -m "project-starter-kit"</kbd> – or use your preferred GUI tool instead). This step is a good idea because it means you will always be able to compare with this first commit to quickly see which code *you've* written as opposed to what came with the starter kit.

5. <kbd>cd</kbd> into your new project, and run <kbd>npm install</kbd>.

If that all finishes without errors, you're good to go.


## Developing your project

Start the development server like this:

```sh
$ npm start
```

The command output should tell you where your dev server is running (the <kbd>Local</kbd> URL) – open this in your browser. (Tip: if you're using [iTerm](../software/iterm-2), you can simply <kbd>CMD+click</kbd> on the URL and it should open in your browser.)

While the dev server is running, you can edit files within <kbd>client</kbd> and your browser should refresh automatically.

The automatic refreshing is done by [BrowserSync](http://www.browsersync.io/), which also magically syncs up scrolling and other events between multiple devices, making it easier to develop with a bunch of phones and tablets on your desk.

Remember to commit often – see the [git workflow](../git-workflow/) guide.


## Building for production

Run this command to do a full production build:

```sh
$ npm run build
```

That will build a deployable copy of your app to the `dist` directory.

## Deploying to the IG web server

There's a deploy task that lets you easily upload the contents of your `dist` folder to the [IG web server].

### First-time preparation

Before you deploy for the first time, you'll need to set your deploy target:

1. Open `gulpfile.babel.js` and find the line `const deployTarget = '';`
2. Set the value to an appropriate location for your project, such as `'features/henry-rollins-profile'`.
    - This is the location (relative to the public web root) where your project will be uploaded.
    - Think of it as the `XXX` in `https://ig.ft.com/XXX/`
    - **Do not** include a leading or trailing slash.
    - See [Naming conventions] for advice on picking a good project name, and for formatting.

### Deploying

```sh
$ npm run deploy
```


<aside>
<p>Remember: you'll generally want to **build** before you deploy. If you want to do both in one line:</p>
<p><kbd>npm run build && npm run deploy</kbd></p>
</aside>

[IG web server]: ../../resources/ig-web-server/
[Naming conventions]: ../naming-conventions
