# Code 401 | Access Control (ACL)

## Class 08 Reading Notes

I. Review, Research, and Discussion

A. When is basic authorization used and when bearer authorization?

- Basic authorization is used to validate a user at sign in, using username and password, encoded with base64.

- Bearer authorizaiton is used to validate a user's right after sign-in to access secure information, and uses a web token for that purpose, requiring the user to sign in only once (per cookie session).

B. What does the JSON Web Token package do?

- The JWT is a system by which a user may be authorized behind the scenes, requiring said user to sign in with his/her credentials only once.

- The JWT has three parts, (a) a header, (b) a payload, where the relevant information is stored, and (c) a secret, which makes up the token's digital signature.

- All three parts are encrypted with base64 and then hashed with 256-bit encryption.

C. What considerations should we make when creating and storing a SECRET?

- A secret should be kept in the .env, so that it doesn't appear in our public code base.

- It should be stored in a cookie in the browser, not in local or session storage.

- The secret should be long and random.

II. Vocabulary

- encryption: "In cryptography, encryption is the process of encoding information. This process converts the original representation of the information, known as plaintext, into an alternative form known as ciphertext. Ideally, only authorized parties can decipher a ciphertext back to plaintext and access the original information" (wikipedia).
- token: a piece of encrypted code that allows a piece of software to verify the identity of its bearer without requiring the bearer to log into the system again.
- bearer: a user with a token.
- secret: the string upon which the digital signature of a token is based and encrypted.
- JSON Web Token: "JSON Web Token is an Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key" (wikipedia).

III. Preview Notes on Role-based Access Control (RBAC)

### [Role-based Access Control: from a Udacity Course called "Intro to Information Security"](https://www.youtube.com/watch?v=C4NP8Eon3cA)

- Which roles exist in my system for an individual user and which rights should each role be granted?

- Users must be assigned one or more roles, and the roles will determine the user's rights of access.

- RBAC is defined after user authentication.

- Becaus the RBAC policy is associated with the role and not the user, the policy does not need to be redefined when an individiual user departs the organization.

- Same for new users, whose roles will define access.

- Principle of least privilege = providing the least number of rights needed for a given job = damage control.

### ["5 Steps to Simple Role-based Access Control"](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

- 2017: 81% of breaches related to hacking were the result of compromised credentials.

- Access and controling it is more complicated than it seems. 

- RBAC has its origins in the 1970s, with the first formal iteration of it dating to 1992.

- RBAC allows for a systematic and repeatable policy of assignation of rights of access.

- Alternatives to RBAC include the following:

  - ACL = access control lists -> defines rights per document, not role.
  - ABAC = attribute-based access control -> bases access on changing attributes, e.g., time of day.

- Implementing RBAC

  - Take an inventory of your systems.
  - Categorize staff and define roles.
  - Assign roles.
  - Avoid making one-time changes.
  - Review your policies.

[<--back](401week2.md)

[<--home-->](../../README.md)
