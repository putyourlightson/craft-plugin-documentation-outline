# Craft CMS Plugin Documentation Outline

What follows is intended to be a reusable documentation outline for [Craft CMS](https://craftcms.com/) plugins. 

While every plugin’s documentation will be unique, it is useful to have a common structure that makes it easy to read and navigate. This documentation outline is displayed on a single page, however it can be split into multiple pages if necessary.

This is a community resource and contributions are welcome through issues or pull requests.





---





# Gamma Plugin for Craft CMS 3

> Add a summary of what the plugin does and how it can help end-users in a few sentences. 

The Gamma plugin provides useful, intelligent, insightful and rather vague functionality to sites running on [Craft CMS](https://craftcms.com/).

It helps end-users by giving them insights into all manner of things, allowing them to make more informed decisions about their website and business.

> Embed an image beneath the text if appropriate. Images should be stored in a folder in the same repository, for example in `/docs/images`.

![Plugin image](./docs/images/gamma-plugin.jpg)

## Contents

> A table of contents containing the top-level headings (H2) makes the documentation easier to navigate. 

- [License](#license)
- [Requirements](#installation)
- [Usage](#usage)
- [Settings](#settings)
- [How It Works](#how-it-works)
- [Roadmap](#roadmap)

## License

> For a commercial license you should state the license and renewal fees.

This plugin requires a commercial license which can be purchased through the Craft Plugin Store.
The license fee is $X plus \$Y per subsequent year for updates (optional).

> For a free license you should state 

This plugin is licensed for free under the MIT License.

## Requirements

> State the required minimum version of Craft and any other dependencies.

This plugin requires Craft CMS 3.0.0 or later.

## Usage

> Installing a plugin is straightforward and doesn’t require more than a single sentence. 

Install the plugin from the Craft Plugin Store in your site’s control panel or manually using composer:

```
composer require putyourlightson/craft-gamma
```

> Provide a description of how to set up the plugin and begin using it. More details of how the plugin works will go in the [How It Works](#how-it-works) section.

Once the plugin is installed, it will begin collecting data about your site straight away. You can view the results and reports in the plugin page in the control panel.

You can output reports in your twig templates using the following tags:

```
{{ craft.gamma.reports }}
```

## Settings

> Explain what each of the plugin settings does.

#### Enable Reporting

Enables the collection of data about the site for generation reports.

#### Detail Level

The level of detail to collect about the site.

- Low : collects site data only.
- Medium : collects site and user data.
- High : collects site, user and interaction data.

> If the plugin comes with a `config.php` file then describe how to use it and explain any settings that are not already explained above.

### Configuration Settings

The plugin comes with a config file for a multi-environment way to set the plugin settings. The config file also provides more advanced plugin configuration settings. To use it, copy the `config.php` to your project’s main `config` directory as `gamma.php` and uncomment any settings you wish to change.

#### Ignore Sites

An array of site IDs to ignore when collecting data.

#### Ignore Users

An array of user IDs to ignore when collecting data.