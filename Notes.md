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


#### Graph
- Adjacency matrix (2D array)
  - 547 Number of Provinces
- Edge List
  - 323 Number of Connected Components in an Undirected Graph

#### Monotonic Queue
- 239 Sliding Window Maximum

#### conversion between char and int
- 752 Open the Lock

```C#
        /* 
             char is internally represented by a number. 
             '0' - '9' are represented by consecutive numbers.
              so the difference between c and '0'is the correspoding intger value of c
         */
        char c1 = '9';
        Console.WriteLine(c1);
        int i1 = c1 - '0'; // 9

        /*
            Convert.ToInt32(char) 
            convert the value of the specified unicode character to the equivalent 32-bit singed integer.
         */
        char c2 = '9';
        int i2 = Convert.ToInt32(c2); // 57

        /*
            Char.GetNumericValue(char) 
            converts the specified numeric Unicode character to a double-precision floating point number.
         */
        char c3 = '9';
        int i3 = (int)Char.GetNumericValue(c3);


        /*
           Converts the value of the signed integer to its equivalent Unicode character. 
        */
        int i4 = 57;
        char c4 = (char)i4; // '9'

        /*
            Convert.ToChar(Int32)
            Converts the value of the specified 32-bit signed integer to its equivalent Unicode character. 
         */
        int i5 = 57;
        char c5 = Convert.ToChar(i5); // '9'
```
