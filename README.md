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

### Making an app, game, or theme
#### Step 1: Clone
To get started, grab the files out of the repo. You can easily do this by running the following command:
```
git clone https://github.com/Nautilus-OS/community.git
```

#### Step 2a: Start working
There are different steps for each section, so please follow carefully.

#### Step 2b: Making a theme
To make a theme, it's fairly easy. First, navigate to `style.css` in the [main repository](https://github.com/Nautilus-OS/NautilusOS) and copy that file into the `themes/[create your author name]/[your project name]/files/` directory.

Once you've done that, you can change anything you would like! To request fonts to be added, you can either use the `@import` statement in CSS, or [request a font be added to the head of the file.](https://nautilus-os.netlify.app/request/)

Finally, create a file

#### Step 2c: Making an app
Making an app is a little bit more complicated, as there are two different kinds of apps.

You can either make an app embedded into the Javascript, or add your app as a separate HTML file with your own styles and scripts.

Simply put your HTML content inside your new HTML file if you're doing an embedded app, just make sure there's no imports in the head, because there is no head.

**Your app will not be supported offline if you decide to make it in another file!**

To request functions be added to the Javascript for embedded applications, fill out the request [here.](https://nautilus-os.netlify.app/request/)

When making a separate file application, create a new file inside of `apps/[make new author folder]/files/index.html`

Now once you're done with that, create an `appinfo.json` file, formatted as the following:

```json
[
  "name": "Your app name here",
  "icon": "fas fa-sun", // Example FontAwesome icon
  "author": "Your name here"
]
```

#### Step 2d: Making a game
Refer to the steps above for app making.

#### Step 3: Deploy
Once you are done with your app, clone the main repository and add in your app. Now initialize a fork, deploy it, and add it into your `info.json` file with the `url` entry.

#### Step 4: Submit
Once you've verified that your code works in tandem with the other code in Nautilus, you're ready to add a pull request. Open a PR on this repository, appending either [APP], [GAME], or [THEME] to the start of the title and adding the respective tag to the PR. Include information about what your app does, what it's used for, etc. We'll check out your app, and eventually merge it into the main community repository.

If your work is not added, check your PR for any messages from maintainers! We'll help you make your app the best it can be.

### Thanks for submitting!
App developers are appreciated by the team, the users, and everyone in between!

## Help
If you need help, please go to [our help form](https://nautilus-os.netlify.app/help/) or contact the developers on discord.

xor - `@_x8rr`

<sup>Please keep in mind that not all developers are on this list, as not everyone wants to be DM'd with inquiries. Thank you.</sup>
