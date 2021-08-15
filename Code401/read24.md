# Hashtables


`Hash `- A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array. `Buckets` - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs. `Collisions` - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

* Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

* the hash function takes a key and returns an integer. We use the integer to determine where the key/value pair should be placed in the array. The hash code is calculated in constant time and writing to an array at one index is O(1) so the hash map has O(1) access.

![hash](https://he-s3.s3.amazonaws.com/media/uploads/0e2c706.png)

* a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.

## collision

A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.
