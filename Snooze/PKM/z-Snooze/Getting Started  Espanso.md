[[Article]]

[Getting Started | Espanso](https://espanso.org/docs/get-started/)

In this section, we will cover the basics of Espanso to quickly get you started. Make sure to [install Espanso](https://espanso.org/install/) before diving into the next sections.

##### For legacy users

If you are coming from a previous Espanso version (≤ 0.7.3), please read the [Migration](https://espanso.org/docs/migration/overview/) section first.

If you followed the installation correctly, Espanso should be running on your computer. For macOS and Windows users, you should now see the Espanso icon on the status bar:

![Espanso icon on Windows](https://espanso.org/assets/images/tray_explain_image_windows-a4482a39604313a2484a7361cacf93f8.png) ![Espanso icon on macOS](https://espanso.org/assets/images/icon_explain_image_macos-79769f4465a5acf312cd2baa1742c443.png)

Linux users can check if Espanso is running by opening a Terminal and running:

At this point, you are ready to use Espanso! Open any typing application (like Notepad or TextEdit) and type `:espanso`, you should see `Hi there!` appear. If you don't see it, please read the troubleshooting section below.

##### Troubleshooting

If you don't see the Espanso icon on macOS or Windows, or if `espanso status` returned `espanso is not running` on Linux, it means Espanso is not currently running on your machine.

Firstly, try starting Espanso again:

-   **For Windows users**: click Espanso from the Start Menu, or click `START_ESPANSO.bat` for Portable mode users.
-   **For macOS users**: click on the Espanso app again. If you see a security warning, please follow the steps described in the [macOS installation](https://espanso.org/docs/install/mac/#problems-you-may-experience) section.
-   **For Linux users**: open a terminal and run `espanso start`

If none of these steps worked, please reinstall Espanso and try again.

## Understanding Matches[​](https://espanso.org/docs/get-started/#understanding-matches "Direct link to heading")

In its most basic form, Espanso detects when you type a **keyword** and **replaces** it while you are typing. These keywords, known as *triggers*, are defined as simple strings. For example, `:date`, `e'`, `signature` and `>>up` are all valid triggers.

![Espanso replaces a trigger with some other text](https://espanso.org/assets/images/new_match_1-e979325325211ce47eadfc789b980651.png)

The *rule* that associates a trigger with the replaced text is called **Match** and is a core concept of Espanso. Matches are very flexible and capable of solving complex tasks. You can learn all about matches in their [documentation](https://espanso.org/docs/matches/basics/) page.

![Espanso&#39;s Match](data:image/png;base64,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)

Espanso ships with very few built-in matches to give you the maximum flexibility, but you can expand its capabilities in two ways: **creating your own custom matches** or **installing packages**. Both of these options allow you to *include* all your code snippets in an app-specific configuration:

$CONFIG/config/vscode.yml

```
filter_title: "Visual Studio Code"extra_includes:  - "../match/_code_snippets.yml"
```

Because the `$CONFIG/match/_code_snippets.yml` file imports both JS and CSS snippets, you will be able to use both of them in VSCode, even though you haven't included the `$CONFIG/match/_js_snippets.yml` and `$CONFIG/match/_css_snippets.yml` directly.

##### tip

Although matches are similar to the concept of *snippets* and *templates* found in other applications, they are not limited to text replacements.

Espanso's matches are more general, associating a *cause* with an *effect*. In their basic form, the cause is the user typing a keyword and the effect is Espanso inserting the replacement. But a match could also be triggered with the search bar or a keyboard shortcut\*, and the effect could be inserting an image, executing a custom script and much more.

\* This is not currently supported, but it's on the roadmap.

## Configuration[​](https://espanso.org/docs/get-started/#configuration "Direct link to heading")

Espanso uses a **file-based configuration** approach, following the Unix philosophy. All configuration files reside in the `espanso` directory, whose location depends on the current OS:

-   Linux: `$XDG_CONFIG_HOME/espanso` (e.g. `/home/user/.config/espanso`)
-   macOS: `$HOME/Library/Application Support/espanso` (e.g. `/Users/user/Library/Application Support/espanso`)
    -   NOTE: when migrating from the previous 0.7.3 version, the configuration directory will be located in `$HOME/Library/Preferences/espanso` for compatibility purposes.
-   Windows: `{FOLDERID_RoamingAppData}\espanso` (e.g. `C:\Users\user\AppData\Roaming\espanso`)

A quick way to find the path of your configuration folder is by using the following command:

> By default, the configuration folder is hidden on most systems. To open it, copy the path of your configuration folder and paste it in the address bar (aka path bar) of your file manager/explorer.

##### info

From now on, we'll refer to the configuration directory as `$CONFIG`. For example, on Windows you'll have `$CONFIG=C:\Users\user\AppData\Roaming\espanso`.

While this folder may contain multiple files, let's now focus on the most important ones. After a fresh installation, the `$CONFIG` directory should be structured as follows:

```
$CONFIG/  config/    default.yml  match/    base.yml
```

As you can see, there are two sub-folders, `config` and `match`, which in turn contain two files, `default.yml` and `base.yml` respectively. Each of them serves a specific purpose:

-   **The files contained in the `match` directory define *WHAT* Espanso should do.** In other words, this is where you should specify all the custom snippets and actions (aka Matches). The `match/base.yml` file is where you might want to start adding your matches, as shown in the following sections. As the number of snippets grows, you might want to *split* your matches over multiple files to make it easier to manage. For example, you might create the `match/emails.yml` file with the snippets you use while writing emails. You can learn all about matches in the [Matches section](https://espanso.org/docs/matches/basics/).
    
-   **The files contained in the `config` directory define *HOW* Espanso should perform its expansions.** In other words, this is were you should specify all Espanso's parameters and options. The `config/default.yml` file defines the options that will be applied to *all applications by default*, unless an *app-specific configuration* is present for the current app. For example, you might want to enable emoji snippets for all apps in the `config/default.yml` file, but disable them when using Slack in the `config/slack.yml` file. You can learn all about configurations in the [Configuration section](https://espanso.org/docs/configuration/basics/).
    

All these files are defined using the widely popular [YAML](https://en.wikipedia.org/wiki/YAML) format.

## Creating your own Matches[​](https://espanso.org/docs/get-started/#creating-your-own-matches "Direct link to heading")

That's enough theory for now, let's start with some action! Let's say you write a lot of emails and you're tired of writing the greetings at the end, so you decide to speed up the process.

We will configure Espanso so that every time you type `:br`, it will be expanded to:

By now you should know that we need to **define a Match**.

With your favourite text editor, open the `$CONFIG/match/base.yml` file, introduced previously in the [Configuration](https://espanso.org/docs/get-started/#configuration) section. You should see something like:

$CONFIG/match/base.yml

```
# espanso match file# For a complete introduction, visit the official docs at: https://espanso.org/docs/# You can use this file to define the base matches (aka snippets)# that will be available in every application when using espanso.# Matches are substitution rules: when you type the "trigger" string# it gets replaced by the "replace" string.matches:  # Simple text replacement  - trigger: ":espanso"    replace: "Hi there!"...
```

We need to define a new Match, so in the `matches:` section, add the following code:

```
  - trigger: ":br"    replace: "Best Regards,\nJon Snow"
```

##### Important

**Make sure to include the indentation**, otherwise it won't be valid YAML syntax. Also, prefer spaces to tabs if possible.

You should get something like:

$CONFIG/match/base.yml

```
# espanso match file# For a complete introduction, visit the official docs at: https://espanso.org/docs/# You can use this file to define the base matches (aka snippets)# that will be available in every application when using espanso.# Matches are substitution rules: when you type the "trigger" string# it gets replaced by the "replace" string.matches:  # Simple text replacement  - trigger: ":espanso"    replace: "Hi there!"  - trigger: ":br"    replace: "Best Regards,\nJon Snow"...
```

All right! After saving the file, Espanso should automatically detect the change and reload your configuration.

Now try to type `:br` anywhere. If you did everything correctly, you should see `Best Regards` appear!

##### Quick Editing

If you are comfortable using the terminal to edit your configurations, you can also run this command:

which spawns an instance of the system-default text editor.

By default it uses Nano on Unix and Notepad on Windows, but you can customize it as you like. Take a look at [Quick Editing](https://espanso.org/docs/configuration/basics/#quick-editing) for more information.

## Understanding Packages[​](https://espanso.org/docs/get-started/#understanding-packages "Direct link to heading")

Custom matches are great, but sometimes it can be tedious to define them for every common operation, especially when you want to **share them with other people**.

Espanso offers an easy way to **share and reuse matches** with other people, **packages**. In fact, they are so important that Espanso includes a **built-in package manager** and a **store**, the [Espanso Hub](https://hub.espanso.org/).

If you are lucky enough, someone might have already written a **package** to include the matches you need! Otherwise, you can create a package and publish it on the Hub, for more information check out the [Packages](https://espanso.org/docs/packages/basics/) documentation.

### Installing a Package[​](https://espanso.org/docs/get-started/#installing-a-package "Direct link to heading")

Let's say you want to **add some emojis** to Espanso, such that when you type `:ok` it gets expanded to 👍.

A solution would be to install the [Basic Emojis](https://hub.espanso.org/basic-emojis) package from the [Espanso Hub](https://hub.espanso.org/) store. Open a terminal and type:

```
espanso install basic-emojis
```

Espanso should detect the change and reload the configuration automatically. If you now type `:ook` into any text field, you should see 👍👍👍👍 appear!

##### Troubleshooting

Espanso should automatically reload the configuration after you install a package. If that doesn't happen, please open a terminal and run:

## Useful shortcuts[​](https://espanso.org/docs/get-started/#useful-shortcuts "Direct link to heading")

Let's conclude this introduction with the most important shortcuts Espanso offers, the **search-bar shortcut**, the **backspace undo** and the **toggle shortcut**.

### Search-bar[​](https://espanso.org/docs/get-started/#search-bar "Direct link to heading")

Espanso comes with a powerful *Search-bar* to quickly find and insert your matches. You can open the search bar in two ways:

-   By pressing `ALT+SPACE` (Option+Space on macOS).
-   By clicking on the status icon and then selecting "Open Search bar" (currently not available on Linux).

If you want to customize the shortcut, please check out the [customizing the Search bar](https://espanso.org/docs/configuration/options/#customizing-the-search-bar) section.

### Backspace Undo[​](https://espanso.org/docs/get-started/#backspace-undo "Direct link to heading")

Sometimes you might accidentally trigger an expansion. If you immediately press the `BACKSPACE` key after the expansion, the action is reverted and the trigger recovered.

You can also disable this behavior by adding the following line on your `config/default.yml` file:

> Note that backspace undo might not be always available.

### Toggle Key[​](https://espanso.org/docs/get-started/#toggle-key "Direct link to heading")

Sometimes you might want to **disable Espanso to avoid an unwanted expansion**. This can be accomplished in many ways, including the icon menu:

![Icon Menu](https://espanso.org/assets/images/icon-menu-505f49d8edc22ab37581ea1feaa57566.png)

If you want a quicker way to toggle Espanso ON and OFF, you can also [Customize the Toggle Key](https://espanso.org/docs/configuration/options/#customizing-the-toggle-key).