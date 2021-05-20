#### List<T>.OrderBy() vs List<T>.Sort()
- list.OrderBy doesn't change the list itself. Instead, it will return an IOrderedEnumerable<T> whose elemenet are sorted.
- list.Sort() will do a in-place sort.
- Problem LC 1329. Sort the Matrix Diagonally

#### IComparable<T> vs IComparer<T>
- IComparable<T>: For a class implemented IComparable, the instances of the class are comparable.
- IComparer<T>: For a class implemented IComparer<T>, the instance of the class can be used to compare two instances of type T.
- Problem LC 295. Find Median from Data Stream

#### module operation
- 1010 Pairs of Songs With Total Durations Divisible by 60
