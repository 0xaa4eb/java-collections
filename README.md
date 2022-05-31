Various fancy collections

## Non-thread safe collections

### Trees and maps

TBD

### Queues

TBD

### Lists

TBD

## Thread-safe collections

TBD

## Persistent collections

| Name                          | Paper | Algorithmic complexity | Implementation                                                                                                                 | Notes                                                                                                                                                                                                                                                   |
|-------------------------------|-------|------------------------|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| PersistentHashArrayMappedTrie | Title | O(k)                   | [grpc library](https://github.com/grpc/grpc-java/blob/master/context/src/main/java/io/grpc/PersistentHashArrayMappedTrie.java) | Delete is not supported, but replacement is. The implementation  favors simplicity and low memory allocation during insertion. Although the asymptotics are good, it is optimized for small sizes like less than 20; "unbelievably large" would be 100. |