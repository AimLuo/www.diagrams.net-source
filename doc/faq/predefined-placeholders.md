---
title: Predefined placeholders
layout: page
faq: true
categories: [Features,Customisation]
---

图表中的每个形状都可以包含元数据或自定义属性 - 关于这些形状的额外信息。

这些自定义属性也可以用于定义占位符值，就像计算机程序中的变量一样。占位符可用于形状标签和工具提示中，以显示该形状的自定义属性值、它所在的容器形状或多组形状中的祖先的值。

了解如何在[标签和工具提示中使用占位符](/blog/placeholders.html)。

## 预定义的占位符

除了使用属性名称作为占位符外，您还可以使用以下预定义的占位符。

|:----- |:----- |
| ``%id%`` |  Prints the ID of a shape or connector. |
| ``%width%`` |  Prints the width of a shape. |
| ``%width:unit%`` |  Prints the width of a shape in the given unit (mm, in, m or current). |
| ``%height%`` |  Prints the height of a shape. |
| ``%height:unit%`` |  Prints the height of a shape in the given unit (mm, in, m or current). |
| ``%length%`` |  Prints the length of a connector. |
| ``%length:unit%`` |  Prints the length of a connector in the given unit (mm, in, m or current). |
| ``%date%`` | Prints the current date using the system locale. |
| ``%time%`` | Prints the current time using the system locale. |
| ``%timestamp%`` | Prints a timestamp using the system locale. |
| ``%date{format}%`` | Prints a timestamp using a custom format, details below. |
| ``%pagenumber[(+|-)n]%`` | Prints the page number of the current page with an optional +/- number expression, eg. %pagenumber-1%. |
| ``%pagecount[(+|-)n]%`` |  Prints the total number of pages with an optional +/- number expression, eg. %pagecount-1%. |
| ``%page%`` | Prints the title of the current page. |
| ``%filename%`` | Prints the name of the file. |

### Placeholders for Atlassian Confluence Server and DC

|:------------|:----|
| ``%version%`` | Prints the current version of the file. |
| ``%creatorName%`` | Prints the name of the user that created the file. |
| ``%lastModifiedBy%`` | Prints the name of the user that last modified the file. |
| ``%lastModifiedTime[:format]%`` |  Prints the last modified time using an optional date format, eg. %lastModifiedTime:dddd, mmmm d, yyyy% |

**Notes:**

* To print some text between ``%`` characters without the text being replaced, use two ``%`` characters. For example, ``%%name%`` prints ``%name%`` even if a property called ``name`` exists.
* If a shape and its ancestor have a property with the same name, the value of the child shape's property is used (this overrides the ancestor property). Likewise, if multiple ancestors have a common property, the value of the closest ancestor's property is used. In this way, [placeholder labels respect scope](/blog/placeholder-scope.html).

## Custom timestamp formats

The following custom formats for timestamps are defined (e.g. ``%date{dddd, mmmm d, yyyy}%``)

| Timestamp format | Description |
|:-----|:------------|
| ``d`` | Day of the month as digits; no leading zero for single-digit days. |
| ``dd`` | Day of the month as digits; leading zero for single-digit days. |
| ``ddd`` | Day of the week as a three-letter abbreviation. |
| ``dddd`` | Day of the week as its full name. |
| ``m`` | Month as digits; no leading zero for single-digit months. |
| ``mm`` | Month as digits; leading zero for single-digit months. |
| ``mmm`` | Month as a three-letter abbreviation. |
| ``mmmm`` | Month as its full name. |
| ``yy`` | Year as last two digits; leading zero for years less than 10. |
| ``yyyy`` | Year represented by four digits. |
| ``h`` | Hours; no leading zero for single-digit hours (12-hour clock). |
| ``hh`` | Hours; leading zero for single-digit hours (12-hour clock). |
| ``H`` | Hours; no leading zero for single-digit hours (24-hour clock). |
| ``HH`` | Hours; leading zero for single-digit hours (24-hour clock). |
| ``M`` | Minutes; no leading zero for single-digit minutes. <br>Uppercase ``M`` unlike CF timeFormat's ``m`` to avoid conflict with months. |
| ``MM`` | Minutes; leading zero for single-digit minutes. <br>Uppercase ``MM`` unlike CF timeFormat's ``mm`` to avoid conflict with months. |
| ``s`` | Seconds; no leading zero for single-digit seconds. |
| ``ss`` | Seconds; leading zero for single-digit seconds. |
| ``l`` _or_ ``L`` | Milliseconds. ``l`` prints 3 digits. ``L`` prints 2 digits. |
| ``t`` | Lowercase, single-character time marker string: ``a`` or ``p``. <br>No equivalent in CF. |
| ``tt`` | Lowercase, two-character time marker string: ``am`` or ``pm``. <br>No equivalent in CF. |
| ``T`` | Uppercase, single-character time marker string: ``A`` or ``P``. <br>Uppercase ``T`` unlike CF's ``t`` to allow for user-specified casing. |
| ``TT`` | Uppercase, two-character time marker string: ``AM`` or ``PM``. <br>Uppercase ``TT`` unlike CF's ``tt`` to allow for user-specified casing. |
| ``Z`` | US timezone abbreviation, e.g. ``EST`` or ``MDT``. With non-US timezones or in the Opera browser, the ``GMT/UTC`` offset is returned, e.g. ``GMT-0500``. <br>No equivalent in CF. |
| ``o`` | GMT/UTC timezone offset, e.g. ``-0500`` or ``+0230``. Note: No equivalent in CF. |
| ``S`` | The date's ordinal suffix (``st``, ``nd``, ``rd``, or ``th``). Works well with ``d``. <br>No equivalent in CF. |
| ``'…'`` _or_ ``"…"`` | Literal character sequence. The surrounding quotes are removed. <br>No equivalent in CF. |
| ``UTC:`` | Must be the first four characters of the timestamp mask. Converts the date from local time to UTC/GMT/Zulu time before applying the time format. <br>The ``"UTC:"`` prefix is removed. <br>No equivalent in CF. |

<br>
### Predefined timestamp formats

There are several predefined timestamp formats that you can use.

| Name | Timestamp format  | Example |
|:---- |:----- |:------- |
| ``default`` | ddd mmm dd yyyy HH:MM:ss | Sat Jun 09 2007 17:46:21 |
| ``shortDate`` | m/d/yy | 6/9/07 |
| ``mediumDate`` | mmm d, yyyy | Jun 9, 2007 |
| ``longDate`` | mmmm d, yyyy | June 9, 2007 |
| ``fullDate`` | dddd, mmmm d, yyyy | Saturday, June 9, 2007 |
| ``shortTime`` | h:MM TT | 5:46 PM |
| ``mediumTime`` | h:MM:ss TT | 5:46:21 PM |
| ``longTime`` | h:MM:ss TT Z | 5:46:21 PM EST |
| ``isoDate`` | yyyy-mm-dd | 2007-06-09 |
| ``isoTime`` | HH:MM:ss | 17:46:21 |
| ``isoDateTime`` | yyyy-mm-dd'T'HH:MM:ss | 2007-06-09T17:46:21 |
| ``isoUtcDateTime`` &nbsp;&nbsp; | UTC:yyyy-mm-dd'T'HH:MM:ss'Z' &nbsp;&nbsp; | 2007-06-09T22:46:21Z |

**Note:** Full and short names for days and months are currently only available in English.
