<p align="center">
  <a href="https://github.com/homebridge/homebridge"><img src="https://raw.githubusercontent.com/homebridge/branding/latest/logos/homebridge-color-round-stylized.png" height="140"></a>
</p>

<span align="center">

# Verified By Homebridge

</span>

The **Verified By Homebridge** program allows plugin developers to get their plugins reviewed and endorsed by the Homebridge project team.

## Benefits

* Have your plugin reviewed by the Homebridge team.
* Increase the visibility of your plugin.
* Increase the level of trust end users place in your plugin.
* The **Verified** shield icon will turn green next to your plugin in the [Homebridge UI](https://github.com/oznu/homebridge-config-ui-x).
* The [**Donate**](https://github.com/oznu/homebridge-config-ui-x/wiki/Developers:-Donation-Links) heart icon will turn pink and enable on your plugin tile in the Homebridge UI.
* Your plugin is bumped to the top of the search results in the Homebridge UI.
* You can optionally upload an icon for your plugin which will be displayed in the Homebridge UI.

## Requirements

The Homebridge project team will check that your plugin meets the following criteria:

- **General**
  - The plugin must be of type [dynamic platform](https://developers.homebridge.io/#/#dynamic-platform-template).
  - The plugin must not offer the same nor less functionality than that of any existing **verified** plugin.
- **Repo**
  - The plugin must be published to NPM and the source code available on a GitHub repository, with issues enabled.
  - A GitHub release should be created for every new version of your plugin, with release notes.
- **Environment**
  - The plugin must run on all [supported LTS versions of Node.js](https://github.com/homebridge/homebridge/wiki/How-To-Update-Node.js), at the time of writing this is Node v18 and v20.
  - The plugin must successfully install and not start unless it is configured.
  - The plugin must not execute post-install scripts that modify the users' system in any way.
  - The plugin must not require the user to run Homebridge in a TTY or with non-standard startup parameters, even for initial configuration.
- **Codebase**
  - The plugin must implement the [Homebridge Plugin Settings GUI](https://developers.homebridge.io/#/config-schema).
  - The plugin must not contain any analytics or calls that enable you to track the user.
  - If the plugin needs to write files to disk (cache, keys, etc.), it must store them inside the Homebridge storage directory.
  - The plugin must not throw unhandled exceptions, the plugin must catch and log its own errors.

These verification requirements were last updated on 2023-12-08. Existing verified plugins will have met the requirements at the time of verification, and not necessarily the current requirements.

## How To Request Verification

If you would like your plugin verified, please open an [issue](https://github.com/homebridge/verified/issues/new/choose) on this repository and fill in the template. The Homebridge project team will then review your plugin and provide constructive feedback if required.

If you feel that your plugin should replace the verification status of an existing plugin, let us know and this will be dealt with on an individual basis.

If you need assistance meeting the verification requirements, please reach out on the [Homebridge Discord](https://discord.gg/A7nCjbz).

## Post Verification

Once your plugin has been verified you will remain in full control of the GitHub repository and npm package. Your plugin will appear on the 'Verified By Homebridge' plugin list and the '**Verified**' badge will appear next to your plugin when the next update to the [Homebridge UI](https://github.com/oznu/homebridge-config-ui-x) is published.

You may optionally add one of the **Verified By Homebridge** badges to your plugin's README:

[![verified-by-homebridge](https://badgen.net/badge/homebridge/verified/purple)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)

```
[![verified-by-homebridge](https://badgen.net/badge/homebridge/verified/purple)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)
```

[![verified-by-homebridge](https://img.shields.io/badge/homebridge-verified-blueviolet?color=%23491F59&style=for-the-badge&logoColor=%23FFFFFF&logo=homebridge)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)

```
[![verified-by-homebridge](https://img.shields.io/badge/homebridge-verified-blueviolet?color=%23491F59&style=for-the-badge&logoColor=%23FFFFFF&logo=homebridge)](https://github.com/homebridge/homebridge/wiki/Verified-Plugins)
```

If you decide you no longer wish to maintain your plugin, please reach out to the Homebridge team on the [Homebridge Discord](https://discord.gg/6GUFCb). We can assist in finding a new owner, or take over the repository until a new maintainer can be found.

## Community

The [#plugin-development](https://discord.gg/A7nCjbz) channel in the official Homebridge Discord server is where Homebridge plugin developers can get tips and advice from other developers and the Homebridge project team.

<span align="center">

[![Homebridge Discord](https://discordapp.com/api/guilds/432663330281226270/widget.png?style=banner2)](https://discord.gg/kqNCe2D)

</span>

## Unverification

Your plugin may be subject to another review or be removed from the verification list when deemed necessary by the Homebridge team - this could be (but not limited to) the following scenarios:

- We notice an increased amount of issues arising from your plugin, which results in a suboptimal experience for the user, for example, a Homebridge crash loop.
- Your plugin has been unmaintained for some time, and a fork or new plugin offering improved functionality is created.

We will generally do our best to contact existing developers of plugins before removing verification status. However, we may **immediately** remove verification status in the following (but not limited to) the following scenarios:

- We notice any sort of user analysis tracking in a verified plugin
- A new plugin requests verification which replaces the functionality of any existing plugin, and we notice that the existing plugin has not been maintained for an extended period of time (and we deem it likely that any contact attempt with the developer would be unsuccessful).

## Credits

- Thanks to [@hjdhjd](https://github.com/hjdhjd) for the *for-the-badge* style badge!
