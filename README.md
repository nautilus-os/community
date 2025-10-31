# Nautilus Community
The official repository for the NautilusOS Community Hub. Home to community-made apps, games, and themes.

## What's in here?
As mentioned above, apps, games, and themes made by people outside of the Nautilus organization are hosted here. All code has been checked by their respective developers and the NautilusOS team.

## File Structure
```text
.
├── README.md
├── LICENSE
├── apps/
│   └── [author name]/
│       ├── [project name]/
│       │     files/
│       │     └── [example.html]
│       │     └── [info.json]
│       └── README.md
├── games/
│   └── [author name]/
│       ├── [project name]/
│       │     files/
│       │     └── [example.html]
│       │     └── [info.json]
│       └── README.md
└── themes/
    └── [author name]/
        └── [project name]/
              files/
              └── [example.css]
              └── [info.json]
```

## For Developers
Making an item for the store? Just follow the instructions below.

## Making an app, game, or theme

### Getting Started
To start, create a new repository on your account, and name it whatever you want your app to be called.


In this repository, you will store your files.

You can now continue to the next section!

### Making a theme
Making a theme is the simplest process.

To start out, grab the base style over from https://github.com/nautilus-os/nautilusos/blob/main/style.css

Now copy the contents and paste it into your theme file, which should be named something like `[themename].css`.

Now, you can modify the styles inside!

### Making an app
A little bit more complicated than themes, but doable!

To get started, create a folder in your repository with the name of your app.

Next, choose your type of application.

#### HTML App
HTML apps are stored in a different directory, have separate JS and CSS, and are not supported offline. Take this into heavy consideration when making an app.

To make an HTML app, simply create a new file called `index.html` to contain all of your scripts, styles, and other content. These files are allowed to have heads and import external scripts, just make sure they aren't harmful. You can also put local CSS and JS files inside your project folder to be used in the HTML.

#### Embedded App
Embedded apps are apps that are typed into the JS, meaning their content is only created when an app launches, unlike how HTML apps are embedded using iframes. Embedded apps are supported by offline builds, but cannot import external scripts or styles. All styles must comply with the themes, meaning you might have to use built in classes and things like that. HTML apps are recommended for flexibility, but if you can work with the provided elements, go for it! Now, you can embed `<script>` tags, but using those are not guaranteed to work or run properly, and can run into errors, so we advise staying away. We also strongly ask that you do not include a head inside your HTML content.

Anyway, you can start writing your app in a separate HTML file under your project folder, and we'll put it in the JS.

### Getting it ready
Now that you have your ready app, you can enter the pre-submit process.

In your app directory (folder), create an appinfo.json file, with the following info:

```json
[
  {
    "name": "",
    "desc": "",
    "icon": "fas fa-icon-here", // MUST USE FONTAWESOME SOLID (images coming soon)
    "author": "",
    "url": "" // not required for themes, we'll get to this in a later step!
  }
]
```

Now that you've filled out your appinfo.json, you can continue to the next step.

### Deploying your app for testing
To deploy your app for testing, we request you put your app on Netlify or Vercel, as Nautilus runs on those two platforms, so we can best get results.

Grab your deployment URL and add that into the `url` slot in your appinfo.json file.

### Submitting
Once you've gone through the whole process, you can finally submit your app! Open an issue, tag it with your content type (app, game, or theme), and fill out the required fields and checkboxes and stuff.

We'll get back to you in about 1-3 days, if not in a few hours, and we'll reply with the next steps or things to change.

## Thanks for contributing!
App developers are appreciated by the team, the users, and everyone in between!

## Help
If you need help, please go to [our help form]([https://nautilus-os.netlify.app/help/](https://nautilus-os.vercel.app/community/help.html)) or contact the developers on discord.

xor (Community Manager) - `@_x8rr`

lane (Developer) - `@scammerseason`

<sup>Please keep in mind that not all developers are on this list, as not everyone wants to be messaged with inquiries. Thank you.</sup>
