# Reading 09 Notes

[Home](README.md)

## Functional Programming Concepts
### What is functional programming?
It is a programming paradigm. It is the style of building the structure and elements of computer programs. 
### Pure programming
This is when it returns the same result
### Immutable data


## Refactoring Javascript for Readability
Examples of Readability in JavaScript:
const friendlyWords = require('friendly-words');

function randomPredicate() {
  const choice = Math.floor(Math.random() * friendlyWords.predicates.length);
  return friendlyWords.predicates[choice];
}

function randomObject() {
  const choice = Math.floor(Math.random() * friendlyWords.objects.length);
  return friendlyWords.objects[choice];
}

async function createUser(email) {
  const user = { email: email };
  user.url = randomPredicate() + randomObject() + randomObject();
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}

It is really easy to read and you know where everything is at and lines up really nice. it is important to not indent too much and make it sloppy. 