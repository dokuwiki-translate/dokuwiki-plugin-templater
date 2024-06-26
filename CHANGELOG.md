# CHANGELOG

2024-05-19:
* removed function getInfo(), [replaced by plugin.info.txt since 2009](https://www.dokuwiki.org/devel:plugin_info).
* removed version numbering (0.8.4 etc): date is better.
* Dealing with [Conflicting Versions and Basenames](https://www.dokuwiki.org/devel:badextensions).

2023-12-14 v0.8.4:
* Rollback: removed `#ifemp`.

2023-12-09 v0.8.3:
* A better fix for "Uninitialized string offset".

2023-12-07 v0.8.2:
* Included Chinese (simplified) translation. (by [粗音未来](miku39@onsei.fans), aka "Miku").

2023-12-06 v0.8.1:
* Fixed "Uninitialized string offset" when user provides "parameter=" without value.

2023-12-05 v0.8:
* Fixed deprecation warning (PageResolver).
* Fixed undefined array keys and other minor errors.
* Implemented `#ifemp` delimiter to hide parameters not provided. (by [Turq Whiteside](https://github.com/TurqW))

2023-08-17 v0.7.1
* Fixed deprecation warning (`require_once(DOKU_PLUGIN.'syntax.php')`).

2023-06-17 v0.7
* Included Dutch translation. (by [Gerrit Uitslag](https://github.com/Klap-in), aka "Klap-in")
* Some modifications to facilitate the translation by DokuWiki Translation Tool.

2023-05-23 v0.6.2
* Previous changes didn't allow the actual displayed string to start or end with quotation marks. This fixes that by allowing such strings to be ""double quoted"" and only removing the outermost quotes. (by [Turq Whiteside](https://github.com/TurqW))

2023-01-03 v0.6.1
* By trimming off quotation marks after the whitespace trim, we allow users to wrap their strings in quotation marks in order to keep any intentional leading or trailing whitespace - useful for bulleted lists, code blocks etc. (by [Turq Whiteside](https://github.com/TurqW))

2022-11-27 v0.6
* Fixed doesn't show the heading when calling just a section.
* Complete rework of function _ _getSection()_.

2022-11-25a v0.5.2
* Better fix for `{{template>page#section}}` doesn't exist with error message.
* Updated error messages to look better.
* Updated english and brazilian portuguese translations.

2022-11-25 v0.5.1
* Internationalization: added lang/en and lang/pt-br.
* Bug fix for when `{{template>page#section}}` doesn't exist.

2022-11-24 v0.5
* Fixed some warnings.
* Doesn't show the heading when calling just a section of a template `{{template>page#section}}`.

2022-11-21 v0.4
* Updated v0.3.1 to work with DokuWiki 2022-07-31 "Igor":
  * Updated functions _handle_ (line 91) and _render_ (line 117).
  * Fixed _array_search()_ warning at line 152. (by [Jack126Guy](https://github.com/jack126guy))
  * Fixed PHP 7+ error (line 171).
  * Fixed PHP curly braces (line 229).
* This is Daniel Dias Rodrigues' first update.

2009-03-21 v0.3.1
* Vincent de Lau's update:
  * Added escaping `|` as `\|`.
  * Trimming keys and variables.
  * Allowing multiple instances of a template and default values (default default = '').

2005-10-26 v0.2
* Changed the substitution delimiters from `{ }` to `@`.
* Perform substitution on parsing rather then on output.
* When the template does not exist show a link to create the template.

2005-10-25 v0.1
* First Version.
