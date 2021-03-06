# Snippets plugin for MantisBT

Copyright (c) 2010 - 2012  John Reese - http://noswap.com  
Copyright (c) 2012 - 2016  MantisBT Team - mantisbt-dev@lists.sourceforge.net

Released under the [MIT license](http://opensource.org/licenses/MIT)


## Description

Define snippets of text that can be easily pasted into text fields


## Requirements

The plugin requires [Mantis](http://www.mantisbt.org/) version 1.3 or higher.

Note that jQuery version 1.6 or later is also required, but since a more recent
version of the library comes bundled with MantisBT, no extra setup is necessary.


## Installation

1. Download or clone a copy of the [plugin's code](https://github.com/mantisbt-plugins/snippets).
2. Copy the plugin (the `Snippets/` directory) into your Mantis
   installation's `plugins/` directory.
3. While logged into your Mantis installation as an administrator, go to
   *Manage -> Manage Plugins*.
4. In the *Available Plugins* list, you'll find the *Snippets* plugin;
   click the **Install** link.
5. In the *Installed Plugins* list, click on the **Snippets** plugin to configure it.


## Usage

### Managing Snippets

- Global snippets can be managed from *Manage -> Manage Plugins*.
- User-specific snippets can be managed from *My Account -> My Snippets*.

The following placeholders are supported in the Snippet's text; they will be
replaced by the corresponding contents when inserted:

 Placeholder | Description
:-----------:|-------------------------
{user}       | your username
{reporter}   | the bug reporter's name
{handler}    | the bug handler's name
{project}    | the project name


### Using Snippets

Each configured text field will have a selection list above it, which can be
used to pick the desired Snippet.

Once selection is made, the Snippet's text will be inserted in the field at the
current position. If text is currently selected, the Snippet will replace the
selection.

By default only the *Bug Note* field is configured to use Snippets.
Other *text* fields (*Description*, *Steps To Reproduce* as well as *Additional
Information*) can be setup to use Snippets via configuration page `Manage > Global Snippets > Configuration`.

## Support

Problems or questions dealing with use and installation should be
directed to the [#mantisbt](irc://freenode.net/mantisbt) IRC channel
on Freenode.

The latest source code can found on
[Github](https://github.com/mantisbt-plugins/snippets).

We encourage you to submit Bug reports and enhancements requests on the
[Github issues tracker](https://github.com/mantisbt-plugins/snippets/issues).
If you would like to propose a patch, do not hesitate to submit a new
[Pull Request](https://github.com/mantisbt-plugins/snippets/compare/).

## MantisBT Versions Supported

- MantisBT v1.3.x - master branch
- MantisBT v1.3.x (modern UI) - modern-ui branch (see https://github.com/mantishub/mantisbt for modern UI)
- MantisBT v1.2.x - master-1.2.x branch

