## Basic Collection Type Attributes and Characterists
You should be able to answer the following questions about each core Collection type

|     | Elements Ordered?   | Allows Duplicates? | Elements Added/Removed in a Certain Order? | Allows Key/Values? |
|-----|---------------------|--------------------|--------------------------------------------|--------------------|
|List | Yes - Numbered Index| Yes                | No                                         | No                 |
|Set  | No                  | No                 | No                                         | No                 |
|Queue| Yes - Placed Order  | Yes                | Yes                                        | No                 |
|Map  | No                  | Yes - Values only  | No                                         | Yes                |


## Specific Collection Type Attributes and Characterists
You should be able to answer the following questions about each Collection implementation provided by Java

| Java Type| Parent Interface Type | Allows null? | Elements Sorted? | Uses hashCode? | Uses compareTo? |
|----------|-----------------------|--------------|------------------|----------------|-----------------|
|ArrayList | List                  | Yes          | No               | No             | No              |
|LinkedList| List and Queue        | Yes          | No               | No             | No              |
|HashSet   | Set                   | Yes          | No               | Yes            | No              |
|TreeSet   | Set                   | No           | Yes              | No             | Yes             |
|HashMap   | Map                   | Yes          | No               | Yes            | No              |
|TreeMap   | Map                   | No           | Yes              | No             | Yes             |
