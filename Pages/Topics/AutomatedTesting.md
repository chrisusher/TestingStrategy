[Home](../../ReadMe.md) » [Automated Testing](./AutomatedTesting.md)

# Automated Testing

## Introduction

This page talks in fair detail of the role of Automated Testing as an effective process within a SDLC.

## Automated Testing should be a first class citizen in any SDLC

To deliver high quality testable code, I think you should be using a "Test-Driven" approach to Software Development.  

**This doesn't mean you write tests after the functionality is implemented.**

I have personally seen TDD have the following desired effects:

- Code is better designed, more readable and better documented.
  - Tests are a form of documentation!
- Code is inevitably easier to test and makes sure testability is considered up-front.
- We have high confidence when raising a Pull Request that we have tested our code as we went along not hoping everything will be ok when we merge.
- Consider the data we expect our classes, methods to be able to handle upfront.

### Humans vs Non-Human Testing

There are types of testing that Humans are very good at.  

There are types of testing that Humans are very bad at doing well over a prolonged period of time.

### Human Testing

Humans are very good at asking the following questions:

- **Did we build the right thing?  I.e. Product Validation.**
- **Is the software design right for the long-term?**
- **Is the User Experience (UX) the most efficient or pleasing to use?**
- **Reviewing the '*-ilities*' of Software.**

  - Machines should test the Software so these properties can be assessed.

    - Does the Software scale?
    - Is the Software testable?  Are there the right entrypoints which mean we can do the most efficient testing?
    - Is the Software available?
    - Is the Software secure?

### Non-Human Testing

Machines are good at measuring the following:

- **Is the Software behaviour correct?**
  - Proving the Software does what we think it should.  Doesn't do what it shouldn't. I.e Verification.

- **Regression Testing of existing behaviour.  Especially through a UI.**

- **Did we build it right?**
  - Did we incur high levels of Tech Debt along the way?
  - Can we write high quality Automated Tests for the right components of the codebase?

- **How does the Software perform under different extreme laboratory conditions?**
  - If we have 000000s rows of data, can we handle this?  How does the Software perform?

- **If we deploy, is existing data corrupted in any unintended way?**
