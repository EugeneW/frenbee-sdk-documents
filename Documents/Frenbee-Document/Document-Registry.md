▶ [[Frenbee Document]]

---

The Document Registry is an independent data or file format used as a registry containing outlines of multiple [[Frenbee Document]]s.

Its content is a list of [[Outline]] and [[Folder]] data of several [[Frenbee Document]]s. A look at the Document Registry lets you grasp an outline of a given item set and identify what items are contained without accessing the [[Frenbee Document]]s.

The Document Registry is mainly created by replicating the attributes of the root elements of [[Frenbee Document]]s. In principle, the [`Id`](Id) attribute indicates that the Document Registry are related to [[Frenbee Document]]s. It is also used as part of [[Frenbee Paged Assets]].

In principle, the Document Registry is represented in XML format in a file or when communicated.

* Default file name: `registry.xml`

> In [[Frenbee Core]], the `DocumentRegistry` class corresponds to the Document Registry. The [[Outline]] of each individual item is represented by the `DocumentLink` class.