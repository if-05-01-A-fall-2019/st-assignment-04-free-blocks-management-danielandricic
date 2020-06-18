Andricic Daniel 3AHIF

## Free Blocks Management

### 1.)

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | 0      |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            | 23456   | 7345   |
|            | 8345345 | 34535  |
|            | 634534  | 154698 |
|            | 3478    | 967    |
|            | 56      | 8657   |

### a.) Five new blocks are allocated

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | 0      |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            | <mark>freed</mark>    | 7345   |
|            | <mark>freed</mark>  | 34535  |
|            | <mark>freed</mark> | 154698 |
|            | <mark>freed</mark>     | 967    |
|            | <mark>freed</mark>     | 8657   |


### b.)The block 22 is freed

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | 0      |
|            | 4589    | 24353  |
|            | 43536   | 98745  |
|            | 718     | 76345  |
|            | 345     | 9877   |
|            | <mark>22</mark>      | 7345   |
|            |  | 34535  |
|            | | 154698 |
|            |     | 967    |
|            |     | 8657   |

### c.) Another 5 blocks are allocated

| Block      | 17      | 18     |
|------------|---------|--------|
| Next Block | 18      | 0      |
|            | <mark>freed</mark>   | 24353  |
|            | <mark>freed</mark>  | 98745  |
|            |  <mark>freed</mark>   | 76345  |
|            |  <mark>freed</mark>   | 9877   |
|            |  <mark>freed</mark>    | 7345   |
|            |  | 34535  |
|            | | 154698 |
|            |     | 967    |
|            |     | 8657   |

### d) Another block is allocated

| Block      | <mark>18</mark>     |
|------------|--------|
| Next Block | 0      |
|            | 24353  |
|            | 98745  |
|            | 76345  |
|            | 9877   |
|            | 7345   |
|            | 34535  |
|            | 154698 |
|            | 967    |
|            |   17   |

### e.) Another three blocks are allocated

| Block      | 18     |
|------------|--------|
| Next Block | 0      |
|            | 24353  |
|            | 98745  |
|            | 76345  |
|            | 9877   |
|            | 7345   |
|            | 34535  |
|            | <mark>freed</mark>  |
|            |  <mark>freed</mark>   |
|            |  <mark>freed</mark>    |

### f) Four blocks(23456,8345345,56 and 634534) are freed
| Block      | <mark>634534</mark>  | 18     |
|------------|---------|--------|
| Next Block | 18      | 0      |
|            |         | 24353  |
|            |         | 98745  |
|            |         | 76345  |
|            |         | 9877   |
|            |         | 7345   |
|            |         | 34535  |
|            |         | 23456  |
|            |         | 8345345|
|            |         | 56     |


### 2.) Given the two memory footprint scenarios for Free Blocks Management as presented in class. State the condition under which the linked list approach uses less space than the bitmap approach.

The LinkedList is especially advantageous for larger memory management, because a bitmap can only be managed statically. Therefore it is limited in its size.
A LinkedList can be managed dynamically.
It can be set to any size and its entries are quickly available for access.

The LinkedList can also allocate less memory than a bitmap when the whole memory (RAM) is almost fully used.
In order to always have enough memory available for the processes, LinkedList releases its unused blocks immediately.
