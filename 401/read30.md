# Hash Tables 

## Vocab list:

- Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

- Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

- Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

- Hashing - Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.

- Collisions - A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.

- Bucket Sizes - Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space.

- set( ) - When adding a new key/value pair to a hashtable: send the key to the hash() method. Once you determine the index of where it should be placed, go to that index. Check if something exists at that index already, if it doesn’t, add it with the key/value pair. If something does exist, add the new key/value pair to the data structure within that bucket.

- get( ) - The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

- has( ) - The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

- keys( ) - The keys() method returns a collection (array) of unique hash keys.

- hash( ) - The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

### Things I want to know more about

- I just want to try these out they seem like they could be very useful.

### Sources

- <https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html>
- <https://www.youtube.com/watch?v=MfhjkfocRR0>

[Back To Home](../README.md)