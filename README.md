Various fancy collections

## Non-thread safe collections

### Trees and maps

| Name              | Paper                                                                                  | Algorithmic complexity | Implementation                                                                                                                                                 | Notes |
|-------------------|----------------------------------------------------------------------------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
| AdaptiveRadixTrie | [ARTful Indexing for Main-Memory Databases](https://db.in.tum.de/~leis/papers/ART.pdf) |                        | [mzheravin/exchange-core](https://github.com/exchange-core/collections/blob/master/src/main/java/exchange/core2/collections/art/LongAdaptiveRadixTreeMap.java) |       |

### Queues

TBD

### Lists

TBD

## Thread-safe collections

### Trees and maps

| Name                          | Paper                                                                 | Algorithmic complexity | Implementation                                                                                                                 | Notes                                                                                                                                                                                                                                                   |
|-------------------------------|-----------------------------------------------------------------------|------------------------|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| PersistentHashArrayMappedTrie | [Ideal hash trees](https://lampwww.epfl.ch/papers/idealhashtrees.pdf) | O(k)                   | [grpc library](https://github.com/grpc/grpc-java/blob/master/context/src/main/java/io/grpc/PersistentHashArrayMappedTrie.java) | Delete is not supported, but replacement is. The implementation  favors simplicity and low memory allocation during insertion. Although the asymptotics are good, it is optimized for small sizes like less than 20; "unbelievably large" would be 100. |

## Persistent collections

| Name                          | Paper                                                                 | Algorithmic complexity | Implementation                                                                                                                 | Notes                                                                                                                                                                                                                                                   |
|-------------------------------|-----------------------------------------------------------------------|------------------------|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| PersistentHashArrayMappedTrie | [Ideal hash trees](https://lampwww.epfl.ch/papers/idealhashtrees.pdf) | O(k)                   | [grpc library](https://github.com/grpc/grpc-java/blob/master/context/src/main/java/io/grpc/PersistentHashArrayMappedTrie.java) | Delete is not supported, but replacement is. The implementation  favors simplicity and low memory allocation during insertion. Although the asymptotics are good, it is optimized for small sizes like less than 20; "unbelievably large" would be 100. |