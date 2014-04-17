If the list view for folders supports sorting, enter the integer value in the `Order` box in the [[Outline window]] to change the display order.

> Compatible items in the [[Aspect window]] are displayed in the sorting order. The default sort is in ascending order.

> It is strongly recommended to assign the numbers using intervals such as 100, 200, 300, etc. when you sort custom items for the first time.  This makes it easier to insert items in the list later.

## Details

When items of the [[Frenbee Document]] are listed in the [[Aspect window]], the display order is sorted using the default sort order as described next.  Generally the items are displayed in the ascending order (smallest first).

You can sort using the default sorting rule for [[Frenbee Document]].  You may also use the GUI to select another sorting rule as necessary.

### How to sort items using default sorting rule

Sort using comparison of items as follows.

1. Compare the Order of [[Outline]] (difference between two numbers).
2. If 1 is the same value, compare Name of [[Outline]].
3. If 2 is the same value, compare [[Id]].

> In [[Frenbee Core]], [[Avatar Aspect]] and [[Document Registry]] use the `DocumentLink` class as link to items. The `DocumentLink` class implements the `IComparable<DocumentLink>` interface and works as above in `DocumentLink.CompareTo` method.  The above shows how the `List<DocumentList>.Sort` method sorts items using the default sorting rule.
