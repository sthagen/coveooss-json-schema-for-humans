# JSON Schema for Humans configuration file

- [1. [Optional] Property JSON Schema for Humans configuration file > description_is_markdown](#description_is_markdown)
- [2. [Optional] Property JSON Schema for Humans configuration file > description_safe_mode](#description_safe_mode)
- [3. [Optional] Property JSON Schema for Humans configuration file > expand_buttons](#expand_buttons)
- [4. [Optional] Property JSON Schema for Humans configuration file > show_breadcrumbs](#show_breadcrumbs)
- [5. [Optional] Property JSON Schema for Humans configuration file > collapse_long_descriptions](#collapse_long_descriptions)
- [6. [Optional] Property JSON Schema for Humans configuration file > collapse_long_examples](#collapse_long_examples)
- [7. [Optional] Property JSON Schema for Humans configuration file > link_to_reused_ref](#link_to_reused_ref)
- [8. [Optional] Property JSON Schema for Humans configuration file > recursive_detection_depth](#recursive_detection_depth)
- [9. [Optional] Property JSON Schema for Humans configuration file > deprecated_from_description](#deprecated_from_description)
- [10. [Optional] Property JSON Schema for Humans configuration file > default_from_description](#default_from_description)
- [11. [Optional] Property JSON Schema for Humans configuration file > copy_css](#copy_css)
- [12. [Optional] Property JSON Schema for Humans configuration file > copy_js](#copy_js)
- [13. [Optional] Property JSON Schema for Humans configuration file > template_name](#template_name)
- [14. [Optional] Property JSON Schema for Humans configuration file > custom_template_path](#custom_template_path)
- [15. [Optional] Property JSON Schema for Humans configuration file > show_toc](#show_toc)
- [16. [Optional] Property JSON Schema for Humans configuration file > examples_as_yaml](#examples_as_yaml)
- [17. [Optional] Property JSON Schema for Humans configuration file > old_anchor_links](#old_anchor_links)
- [18. [Optional] Property JSON Schema for Humans configuration file > markdown_options](#markdown_options)
- [19. [Optional] Property JSON Schema for Humans configuration file > template_md_options](#template_md_options)
  - [19.1. [Optional] Property JSON Schema for Humans configuration file > template_md_options > badge_as_image](#template_md_options_badge_as_image)
  - [19.2. [Optional] Property JSON Schema for Humans configuration file > template_md_options > show_heading_numbers](#template_md_options_show_heading_numbers)
  - [19.3. [Optional] Property JSON Schema for Humans configuration file > template_md_options > show_array_restrictions](#template_md_options_show_array_restrictions)
  - [19.4. [Optional] Property JSON Schema for Humans configuration file > template_md_options > properties_table_columns](#template_md_options_properties_table_columns)
    - [19.4.1. JSON Schema for Humans configuration file > template_md_options > properties_table_columns > properties_table_columns items](#autogenerated_heading_2)
- [20. [Optional] Property JSON Schema for Humans configuration file > with_footer](#with_footer)
- [21. [Optional] Property JSON Schema for Humans configuration file > footer_show_time](#footer_show_time)
- [22. [Optional] ~~Property JSON Schema for Humans configuration file > allow_html_description~~](#allow_html_description)
- [23. [Optional] ~~Property JSON Schema for Humans configuration file > minify~~](#minify)
- [24. [Optional] ~~Property JSON Schema for Humans configuration file > templates_directory~~](#templates_directory)

**Title:** JSON Schema for Humans configuration file

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |

**Description:** Choose how to generate JSON Schema for Humans documentation file.

Configuration parameters can be provided in several ways:

- On the CLI using `--config parameter_name=value` (example: `--config template_name=flat`)
- On the CLI using a config file `--config-file config.json`
- From code, by providing a GenerationConfiguration object to the called generation method.

<details>
<summary>
<strong> <a name="description_is_markdown"></a>1. [Optional] Property JSON Schema for Humans configuration file > description_is_markdown</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** (HTML outputs only)
Whether to consider the description as Markdown and render it accordingly.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="description_safe_mode"></a>2. [Optional] Property JSON Schema for Humans configuration file > description_safe_mode</strong>  

</summary>
<blockquote>

|             |                            |
| ----------- | -------------------------- |
| **Type**    | `enum (of null or string)` |
| **Default** | `"escape"`                 |

**Description:** (HTML outputs only)
(Only used with `description_is_markdown`)
How are HTML tags in descriptions handled. Correspond to the `safe_mode` option of the markdown2 library.

- "escape": Escape all HTML tags in descriptions
- "replace": Replace HTML tags with `[HTML_REMOVED]`
- null: Allow HTML in descriptions

Must be one of:
* null
* "escape"
* "replace"

</blockquote>
</details>

<details>
<summary>
<strong> <a name="expand_buttons"></a>3. [Optional] Property JSON Schema for Humans configuration file > expand_buttons</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** Add an `Expand all` and a `Collapse all` button at the top of the generated documentation.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="show_breadcrumbs"></a>4. [Optional] Property JSON Schema for Humans configuration file > show_breadcrumbs</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** For each property, show the relative place of that property in the schema.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="collapse_long_descriptions"></a>5. [Optional] Property JSON Schema for Humans configuration file > collapse_long_descriptions</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** If a description is considered big, show only the beginning and add a `Read more` button.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="collapse_long_examples"></a>6. [Optional] Property JSON Schema for Humans configuration file > collapse_long_examples</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** If an example is considered big, collapse it, it can be displayed with a `Show` option.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="link_to_reused_ref"></a>7. [Optional] Property JSON Schema for Humans configuration file > link_to_reused_ref</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** If several `$ref` points to the same definition, only render the documentation for this definition the first time. All other occurrences are replaced by an anchor link to the first occurrence. The first occurrence is the one that is the least nested from the top of the schema and appears first in that nesting level.

*Note*: If this option is off and the schema contains recursive definitions, the generation will crash!

</blockquote>
</details>

<details>
<summary>
<strong> <a name="recursive_detection_depth"></a>8. [Optional] Property JSON Schema for Humans configuration file > recursive_detection_depth</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `integer` |
| **Default** | `25`      |

**Description:** *Advanced option*
If `link_to_reused_ref` is false and a `$ref` in the schema refers to a parent of itself, we would get a `RecursionError` trying to render the documentation. To avoid this, each reference is checked for circular references.

This option determines the number of times to recursively follow definitions looking for a circular reference.

In other words, if a schema has a deeply nested element that refers to itself, this option may need to be increased.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="deprecated_from_description"></a>9. [Optional] Property JSON Schema for Humans configuration file > deprecated_from_description</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** Mark a property as deprecated (with a big red badge) if the description contains the string `[​Deprecated`.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="default_from_description"></a>10. [Optional] Property JSON Schema for Humans configuration file > default_from_description</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** Extract the default value of a property from the description like this: ``[Default `the_default_value`]``.

The default value from the "default" attribute will be used in priority.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="copy_css"></a>11. [Optional] Property JSON Schema for Humans configuration file > copy_css</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** Copy `schema_doc.css` to the same directory as `RESULT_FILE` after generation.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="copy_js"></a>12. [Optional] Property JSON Schema for Humans configuration file > copy_js</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** Copy `schema_doc.min.js` to the same directory as `RESULT_FILE` after generation.

This file contains the logic for the anchor links.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="template_name"></a>13. [Optional] Property JSON Schema for Humans configuration file > template_name</strong>  

</summary>
<blockquote>

|             |                    |
| ----------- | ------------------ |
| **Type**    | `enum (of string)` |
| **Default** | `"js"`             |

**Description:** The name of the built-in template to use to render the documentation.

`js` is the default and uses javascript for anchor links, collapsible sections and tabs.

`js_offline` is identical to `js` except that all CSS, fonts and JavaScript are bundled for offline use.

`flat` uses no javascript, but has no interactivity.

`md` is the markdown template.

`md_nested` is the markdown template with collapsible nested sections.

Must be one of:
* "flat"
* "js"
* "js_offline"
* "md"
* "md_nested"

</blockquote>
</details>

<details>
<summary>
<strong> <a name="custom_template_path"></a>14. [Optional] Property JSON Schema for Humans configuration file > custom_template_path</strong>  

</summary>
<blockquote>

|             |          |
| ----------- | -------- |
| **Type**    | `string` |
| **Default** | `null`   |

**Description:** Path to a custom Jinja2 template file.

There can be multiple files to split the template, but this path should be the entry point.

If no output file is specified, the extension of the template file will be used to determine the output documentation extension. i.e. if the template is in ./custom_template/content.html, the resulting documentation will have the html extension.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="show_toc"></a>15. [Optional] Property JSON Schema for Humans configuration file > show_toc</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** Whether to render table of contents.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="examples_as_yaml"></a>16. [Optional] Property JSON Schema for Humans configuration file > examples_as_yaml</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** Whether to display examples as YAML instead of JSON

</blockquote>
</details>

<details>
<summary>
<strong> <a name="old_anchor_links"></a>17. [Optional] Property JSON Schema for Humans configuration file > old_anchor_links</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** Generate HTML ids for anchor links without special characters (keep only letters, digits, `_`, and `-`).

This is the old behaviour and is only needed for browsers that do not support HTML 5.

</blockquote>
</details>

<details>
<summary>
<strong> <a name="markdown_options"></a>18. [Optional] Property JSON Schema for Humans configuration file > markdown_options</strong>  

</summary>
<blockquote>

|                           |                                                                                                                                     |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                            |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)                                                         |
| **Default**               | `{"fenced-code-blocks": {"cssclass": "highlight jumbotron"}, "tables": null, "breaks": {"on_newline": true, "on_backslash": true}}` |

**Description:** (Only used with `description_is_markdown`)
[Markdown 2 options](https://github.com/trentm/python-markdown2/wiki/Extras) for the descriptions.

**Example:**

```json
{
    "fenced-code-blocks": {
        "cssclass": "highlight jumbotron"
    },
    "tables": null,
    "break-on-newline": true,
    "cuddled-lists": true
}
```

</blockquote>
</details>

<details>
<summary>
<strong> <a name="template_md_options"></a>19. [Optional] Property JSON Schema for Humans configuration file > template_md_options</strong>  

</summary>
<blockquote>

|                           |                                                                             |
| ------------------------- | --------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                    |
| **Additional properties** | ![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green) |

**Description:** specific options to md template

<details>
<summary>
<strong> <a name="template_md_options_badge_as_image"></a>19.1. [Optional] Property JSON Schema for Humans configuration file > template_md_options > badge_as_image</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `false`   |

**Description:** if true generate badges(eg: optional, required) using embedded image (https://img.shields.io).

 if false, use text instead

</blockquote>
</details>

<details>
<summary>
<strong> <a name="template_md_options_show_heading_numbers"></a>19.2. [Optional] Property JSON Schema for Humans configuration file > template_md_options > show_heading_numbers</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** if true generate heading numbers to correspond to table of contents.

 if false, do not generate heading numbers

</blockquote>
</details>

<details>
<summary>
<strong> <a name="template_md_options_show_array_restrictions"></a>19.3. [Optional] Property JSON Schema for Humans configuration file > template_md_options > show_array_restrictions</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** if true generate array restrictions section.

 if false, do not generate

</blockquote>
</details>

<details>
<summary>
<strong> <a name="template_md_options_properties_table_columns"></a>19.4. [Optional] Property JSON Schema for Humans configuration file > template_md_options > properties_table_columns</strong>  

</summary>
<blockquote>

|          |                             |
| -------- | --------------------------- |
| **Type** | `array of enum (of string)` |

**Description:** array of column names to display in the properties table.

 if empty, the default is ['Property','Pattern','Type','Deprecated','Definition','Title/Description']

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be                                                       | Description |
| ------------------------------------------------------------------------------------- | ----------- |
| [properties_table_columns items](#template_md_options_properties_table_columns_items) | -           |

#### <a name="autogenerated_heading_2"></a>19.4.1. JSON Schema for Humans configuration file > template_md_options > properties_table_columns > properties_table_columns items

|          |                    |
| -------- | ------------------ |
| **Type** | `enum (of string)` |

Must be one of:
* "Property"
* "Pattern"
* "Type"
* "Deprecated"
* "Definition"
* "Title/Description"

</blockquote>
</details>

</blockquote>
</details>

<details>
<summary>
<strong> <a name="with_footer"></a>20. [Optional] Property JSON Schema for Humans configuration file > with_footer</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** Whether to show the footer linking to the library repo and with the generation datetime

</blockquote>
</details>

<details>
<summary>
<strong> <a name="footer_show_time"></a>21. [Optional] Property JSON Schema for Humans configuration file > footer_show_time</strong>  

</summary>
<blockquote>

|             |           |
| ----------- | --------- |
| **Type**    | `boolean` |
| **Default** | `true`    |

**Description:** Whether the footer should display the generation time

</blockquote>
</details>

<details>
<summary>
<strong> <a name="allow_html_description"></a>22. [Optional] ~~Property JSON Schema for Humans configuration file > allow_html_description~~</strong>  

</summary>
<blockquote>

|                |           |
| -------------- | --------- |
| **Type**       | `boolean` |
| **Deprecated** |
| !              | [         | D | e | p | r | e | c | a | t | e | d | ] | ( | h | t | t | p | s | : | / | / | i | m | g | . | s | h | i | e | l | d | s | . | i | o | / | b | a | d | g | e | / | D | e | p | r | e | c | a | t | e | d | - | r | e | d | ) |
| **Default**    | `false`   |

**Description:** [Deprecated]

</blockquote>
</details>

<details>
<summary>
<strong> <a name="minify"></a>23. [Optional] ~~Property JSON Schema for Humans configuration file > minify~~</strong>  

</summary>
<blockquote>

|                |           |
| -------------- | --------- |
| **Type**       | `boolean` |
| **Deprecated** |
| !              | [         | D | e | p | r | e | c | a | t | e | d | ] | ( | h | t | t | p | s | : | / | / | i | m | g | . | s | h | i | e | l | d | s | . | i | o | / | b | a | d | g | e | / | D | e | p | r | e | c | a | t | e | d | - | r | e | d | ) |
| **Default**    | `true`    |

**Description:** [Deprecated]

</blockquote>
</details>

<details>
<summary>
<strong> <a name="templates_directory"></a>24. [Optional] ~~Property JSON Schema for Humans configuration file > templates_directory~~</strong>  

</summary>
<blockquote>

|                |          |
| -------------- | -------- |
| **Type**       | `string` |
| **Deprecated** |
| !              | [        | D | e | p | r | e | c | a | t | e | d | ] | ( | h | t | t | p | s | : | / | / | i | m | g | . | s | h | i | e | l | d | s | . | i | o | / | b | a | d | g | e | / | D | e | p | r | e | c | a | t | e | d | - | r | e | d | ) |

**Description:** [Deprecated]

</blockquote>
</details>

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans)