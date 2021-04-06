## ArrayList methods to Know

| Method        | Return Type          | Parameters                            |
|---------------|----------------------|---------------------------------------|
|add()          | boolean              | (E element) or (int index, E element) |
|remove()       | boolean or E         | (Object object) or (int index)        |
|set()          | E                    | (int index, E newElement)             |
|isEmpty()      | boolean              | none                                  |
|size()         | int                  | none                                  |
|clear()        | void                 | none                                  |
|contains()     | boolean              | (Object object)                       |
|equals()       | boolean              | (Object object)                       |


## List methods to Know

| Method        | Return Type          | Parameters                            |
|---------------|----------------------|---------------------------------------|
|add()          | boolean              | (E element) or (int index, E element) |
|remove()       | boolean or E         | (Object object) or (int index)        |
|isEmpty()      | boolean              | none                                  |
|size()         | int                  | none                                  |
|clear()        | void                 | none                                  |
|contains()     | boolean              | (Object object)                       |
|removeIf()     | boolean              | (Predicate<? super E> filter)         |
|forEach()      | void                 | (Consumer<? super T> action)          |
|replaceAll()   | void                 | (UnaryOperator<E> op)                 |


## Creating Lists

| Method                | Info                            | Add Elements?| Remove Elements? | Replace Elements? |
|-----------------------|---------------------------------|--------------|------------------|-------------------|
|Arrays.asList(varargs) | Fixed size list                 | No           | No               | Yes               |
|List.of(varargs)       | Immutable                       | No           | No               | No                |
|List.copyOf(collection)| Immutable with given collection | No           | No               | No                |
