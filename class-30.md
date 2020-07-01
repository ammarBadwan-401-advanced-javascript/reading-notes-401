# Hashtables

* Terminology:
1. Hash: its the result of algorithm taking a string and convertingit into a value.
2. Buckets: Bucket is whats contained in each index of array.
3. Collisions: it happens when more than one key gets hashed into the same location.

* Why use hashes?

1. Hold unique values.
2. Dictionary.
3. Library

## Structure

### Hashing 

* Hash code turns a key into an integer. It’s very important that hash codes are deterministic: output is determined only by input.

### Creating a Hash

* Hashtables are created from arrays with size of 1024 then use some logic to turn it into numeric value.

We can do that by:
1. Add or multiply all ASCII values.
2. Multiply it by a prime number.
3. Insert into the array at that index.

### Collisions

* Collision happens when more than one key hashes the same index in an array.

* Hash map should be able to handle two keys resolving same index.

### Internal Method 

1. Add() sends a key to gethash method
2. Find() takes a key gets the hash and goes to the index.
3. Contains() takes a key and return a boolean if that key exists.
4. GetHash() accepts a akey as string and conducts the hash.