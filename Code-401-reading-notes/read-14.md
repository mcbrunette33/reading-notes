## Read 14

### Hash Passowrds

- The irreversible mathematical properties of hashing make it a phenomenal mechanism to conceal passwords at rest and in motion. Another critical property that makes hash functions suitable for password storage is that they are deterministic.

- To integrate hashing in the password storage workflow, when the user is created, instead of storing the password in cleartext, we hash the password and store the username and hash pair in the database table. When the user logs in, we hash the password sent and compare it to the hash connected with the provided username. If the hashed password and the stored hash match, we have a valid login. 

- The core purpose of hashing is to create a fingerprint of data to assess data integrity.

- A hashing function takes arbitrary inputs and transforms them into outputs of a fixed length.

- To qualify as a cryptographic hash function, a hash function must be pre-image resistant and collision resistant.

- Due to rainbow tables, hashing alone is not sufficient to protect passwords for mass exploitation. To mitigate this attack vector, hashing must integrate the use of cryptographic salts.

- Password hashing is used to verify the integrity of your password, sent during login, against the stored hash so that your actual password never has to be stored.

- Not all cryptographic algorithms are suitable for the modern industry. At the time of this writing, MD5 and SHA-1 have been reported by Google as being vulnerable due to collisions. The SHA-2 family stands as a better option.

## bcrypt

- Using a Key Factor, BCrypt is able to adjust the cost of hashing. With Key Factor changes, the hash output can be influenced. In this way, BCrypt remains extremely resistant to hacks, especially a type of password cracking called rainbow table.

- If you have sensitive data or information that you need to be protected, ensuring it is secured correctly is vital. As we have seen, there are many ways to secure this information through various password methods, but only BCrypt offers a truly robust solution.

## jbCrypt

- This system hashes passwords using a version of Bruce Schneier's Blowfish block cipher with modifications designed to raise the cost of off-line password cracking and frustrate fast hardware implementation. The computation cost of the algorithm is parametised, so it can be increased as computers get faster. The intent is to make a compromise of a password database less likely to result in an attacker gaining knowledge of the plaintext passwords

- jBCrypt is licensed under a ISC/BSD licence and ships with a set of JUnit unit tests to verify correct operation of the library and compatibility with the canonical C implementation of the bcrypt algorithm.