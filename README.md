# Security with bcrypt

This assignment will allow you to play around with the `bcrypt` package

## Tasks

## Task 1 - getting bcrypt

1. Install the `bcrypt` npm package with `npm i bcrypt`

2. Import `bcrypt` into your `server.js` file

## Task 2 - documentation

Familiarise yourself with the [bcrypt documentation](https://www.npmjs.com/package/bcrypt)

- How do you use it?
- What things can you do with it?

## Task 3 - writing a hashing helper function

> `bcrypt.hash(myPlaintextPassword, saltRounds)`

Write a function which takes a string as an argument, and uses `bcrypt` to hash the result and return the result. Use `10` as the number of salt rounds.

> Note: This method returns a promise, so you might want to use `async / await` or use `.then()`

Test your function by using `console.log()` to display the output

## Task 4 - playing with salt

Play around with the `saltRounds`. Use small and large numbers.

 - How long does the program take to run?
 - What would an ideal `saltRounds` number be?

## Task 5 - writing a compare helper function

> `bcrypt.compare(myPlaintextPassword, hash)`

Write a function which takes 2 strings as an argument.

The first string is your plain text password, and the second string is the hashed version of it (you can generate this with the helper function you wrote in Task 3)

Test your function by using `console.log()` to display the output

What happens if the password you use does not match the hashed version of that password?