XML Search Engines Exporter/Importer (XSEEI)
--------------------------------------------

A lightweight, XUL-based (a.k.a. "legacy") add-on for the Mozilla Firefox web browser to import and export your installed search engines (sometimes called "search plugins") from and to XML files in the OpenSearch format.


### Install

#### Firefox 45 to 56
The latest public release can be still installed from the [archived page of the add-on in addons.mozilla.org (AMO)](https://addons.mozilla.org/addon/search-engines-export-import).


#### Firefox 57 and later
Being a legacy add-on, it can't be installed in Firefox 57 (a.k.a Firefox Quantum) and later versions, where only add-ons built using the WebExtensions model are accepted. Sadly, it's [not possible yet to port this add-on to WebExtensions](https://github.com/nohamelin/xseei/issues/1).

As an alternative, I rewrote the main functions of the add-on as single-file scripts that can be run manually via the Scratchpad Firefox tool.
These scripts work locally and they don't depend on any online service (no data is send to any remote network):

* [xseei.import.js](https://gist.github.com/nohamelin/8e2e1b50dc7d97044992ae981487c6ec): to import search engines.
* [xseei.export-all.js](https://gist.github.com/nohamelin/6af8907ca2dd90a9c870629c396c9521): to export all your search engines to a single ZIP file.

Check the initial comments inside each file for further information.


##### What about Pale Moon, Waterfox and other Firefox forks still supporting XUL-based add-dons?

I haven't tested the add-on with these applications, and I haven't planned to actively support them in future releases. Reports from users trying the add-on with these are welcome, though.


### Resources

* [Creating OpenSearch plugins for Firefox | Mozilla Developer Network](https://developer.mozilla.org/en-US/Add-ons/Creating_OpenSearch_plugins_for_Firefox)
* [The specification of the OpenSearch description format](http://www.opensearch.org/Specifications/OpenSearch/1.1#OpenSearch_description_document)
* [*What about search hijacking?*](http://blog.queze.net/post/2015/11/02/What-about-search-hijacking) it presents the main upstream motivations to get rid of the XML-based storage system for search engines from Firefox.


### Contact

* Questions and bug reports are tracked in the [issues](https://github.com/nohamelin/xseei/issues) page. You will need to have a GitHub account to post here. Alternatively, there is a [thread in the MozillaZine forums](http://forums.mozillazine.org/viewtopic.php?f=48&t=3020165) open to general discussion.
* Translations has been managed via the [Crowdin](https://crowdin.com/project/xseei) platform. These were kindly provided by volunteers.


### License

All the source code is shared under the terms of the [Mozilla Public License (MPL) 2.0](http://www.mozilla.org/MPL/2.0/).
