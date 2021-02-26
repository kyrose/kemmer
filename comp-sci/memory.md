# Computer memory

## Table of the key differences between stack and heap

| **Parameter**           | **Stack**                                 | **Heap**                                                                     |
| ----------------------- | ----------------------------------------- | ---------------------------------------------------------------------------- |
| Data structure          | linear                                    | hierarchical                                                                 |
| Access speed            | fast                                      | slower                                                                       |
| Space management        | managed by OS, never fragments            | Memory can become fragmented as blocks of memory allocated earlier are freed |
| Access                  | Local variables                           | Global variables                                                             |
| Space size limit        | dependent on OS                           | no specific limit                                                            |
| Resizing                | Variables cannot be resized               | Variables resizable                                                          |
| Memory allocation       | In contiguous block                       | Randomly                                                                     |
| Allocation/deallocation | Done automatically by compiler            | Manually by programmer                                                       |
| Deallocation            |                                           | Explicit deallocation required                                               |
| Implementation          | simple array, dynamic memory, linked list | array, trees                                                                 |
| Main issues             | Shortage of memory                        | Memory fragmentation                                                         |
| Flexibility             | Fixed                                     | Resizable                                                                    |                        |                                           |                                                                              |
