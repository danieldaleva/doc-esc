`<esc-button>` #[esc-button]
================================================================================
## Table of Contents

- [Overview](#overview)
- [Sintax](#sintax)
- [Attributes](#attributes)

Overview
--------------------------------------------------------------------------------

The **XML \<esc-button\>** element provides a clickable element, which can be used in forms, or anywhere that needs a simple, standard button functionality. It may display text, icons, or both. A button can be handled and styled with several attributes to behave and look in a specific way.


Sintax
--------------------------------------------------------------------------------

```XML
<esc-button>
  [<esc_name>string</esc_name>]
  [<esc_enabled>boolean</esc_enabled>]
  [<esc_selection_type>enum</esc_selection_type>]
  [<esc_value>string</esc_value>]
  [<esc_label>dom</esc_label>]
  [<esc_icon class="string">string</esc_icon>]
  [<esc_type>enum</esc_type>]
  [<esc_style>enum</esc_style>]
  [<esc_orientation>enum</esc_orientation>]
  [<esc_decoration>
  	[<esc_status>enum</esc_status>]
  	[<esc_content>string</esc_content>]
  </esc_decoration>]
  [<esc_on_selects>
    <esc_on_select>string</esc_on_select>
  </esc_on_selects>]
  [<esc_selectables>
    <esc_selectable>string</esc_selectable>
  </esc_selectables>]
  [<esc_on_destroys>
    <esc_on_destroy>string</esc_on_destroy>
  </esc_on_destroys>]
</esc-button>
```

Attributes
--------------------------------------------------------------------------------

### `[<esc_name>]`

The **esc_name** element adds the `name` attribute to the final rendered button.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_name** |
|  Required  | no |
|  Type  | string |

<br/>

### `[<esc_enabled>]` 

The **esc_enabled** element adds the `enabled` attribute to the final rendered button.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_enabled** |
|  Required  | no |
|  Type  | boolean |
|  Value  | `true \| false` |


<br/>

### `[<esc_type>]`

The **esc_type** element set the style to the button shape:
* **shaded filled** ``strong``,
* **outline filled** ``ghost`` and
* **clear filled** ``subtle``.

The default value is `strong`.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_type** |
|  Required  | no |
|  Type  | enum |
|  Value  | `strong \| ghost \| subtle` |
|  Default  | `strong` |

<br/>

### `[<esc_style>]`

The **esc_style** element set the font style modes to the button label:
* **bold** ``regular`` and
* **light** ``light``.

The default value is `regular`.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_style** |
|  Required  | no |
|  Type  | enum |
|  Value  | `regular \| light` |
|  Default  | `regular` |

<br/>

### `[<esc_orientation>]`

The **esc_style** element set the orientation style to the button label:
* **horizontal** ``horizontal`` and
* **vertical** ``vertical``.

The default value is `horizontal`.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_orientation** |
|  Required  | no |
|  Type  | enum |
|  Value  | `horizontal \| vertical` |
|  Default  | `horizontal` |

<br/>

### `[<esc_on_selects>]`

The **esc_on_selects** element adds the behavior on button click. It accepts javascript.

| Label | Description |
| --- | --- | 
|  Attribute   | **esc_on_selects** |
|  Required  | no |
|  Value  | \<esc_on_select\> |

 - ### `<esc_on_select>`

   The **esc_on_select** element adds the `onClick` event to the rendered button. It returns the Event object and accepts pure javascript as string to handle the event data.  

   | Label | Description |
   | --- | --- | 
   |  Attribute   | **esc_on_select** |
   |  Required  | yes |
   |  Value  | string |
