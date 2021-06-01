# Hash Table

- to hash is to input a string into while algorithmically adding information to the value for use in more effeciently locatin gthe value in subsequent searches.
- Buckets - are what contain the hashed values, which my or may not includ multiple value pairs due to collisions
- Collisions when a value after being hashed attempt to select an already occupied bucket.
- Every bucket has a key value pair
- each hash must be unique and decodable, not random
  ### some methods include:
  - Add or multiply all the ASCII values together.
  - Multiply it by a prime number such as 599.
  - Use modulo to get the remainder of the result, when divided by the total size of the array.
  - Insert into the array at that index.

- when a value happends to match another, it will move the new vale into a linked list.
- with this added layer of information that can be determined only using the input value searches can be made much faster.