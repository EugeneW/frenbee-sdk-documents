▶ [[Frenbee Document]] ▶ [[Types|Frenbee Document#types]]

---

CSV (Comma Separated Values) is a notation method that the Frenbee system uses to enumerate the values of multiple string representations in HTTP request parameter, XML attributes, etc. Generally, the CSV format has some variations. Frenbee uses the format described below.

* Values are separated by `,` with no nonnumeric blank character put immediately before or after it. (This is to reduce the amount of information to be processed and ensure simple analysis processing.)
* A value that contains `,`, `"`, or a newline code is handled as follows.
* Multiple lines of data are represented by using a newline outside a value (`\r`, `\n`, or `\r\n` in C (C#) representation).

> In C# code, the whole CSV data is handled as string type data or each value on one line of CSV data is handled as string[] type data.

## When encoding CSV
* A value containing any CSV control character (`,`, `"`, `\r`, or `\n`) in C (C#) representation must be enclosed in `"`.
(The alternative is not to enclose it in double quotes in order to ensure readability comparable to that of simple CSV used for development and reduce the amount of information.)
* In C (C#) representation, replace (encode) `\"` in values with `\"\"`. In other words, replace `"` in values with `""`.

### Reference

> A CSV representation in an HTTP query is percent-encoded. For example, `"` is encoded to `%22`.

> When a CSV representation is included in XML code, `"` is encoded to `&quot;`, for example.

## Supplement

In actual use, when a high level of representation is not required, the functions may be limited as described below.

* When encoding is not supported (called "simple CSV" in the case of Frenbee)
* When only single lines are supported (use of multiple-line data is not specified)

> When [[CSV]] fields of Untiy Editor are edited, representation may be limited to [[CSV text field]].
