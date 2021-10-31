# This repo is a replay of https://github.com/mjhea0/flaskr-tdd

# Test case for group project: https://github.com/ECE444-2021Fall/project1-education-pathways-group-15-apricot-studios/blob/Jiaxing_Lab6_TDD/flask-app/tests/app_test.py#L40-L63

# What are the pros and cons of TDD?

## Pros
* Tests are written before the actual implementation. This means the requirements for each unit are clear.
* TDD ensures safer refactoring. Since tests make sure input/output (or interface) of a module works as expected, tests can check the results of the internal implementation refactoring.
* TDD encourages modularization by its nature. This improves maintainability of the code.
* Having testing as an important part of development yields better code quality.
* Tests provide good documentations by themselves. They demonstrate how a module is expected to be used.
* TDD makes team collaboration easier. Developers can confidently change others' code with the verification from tests.

## Cons
* Tests themselves need to be written and maintained by developers, creating overheads and potentially slow down the development.
* TDD is hard to be implemented in legacy code especially when legacy code is not modularized.
* Relying too much on tests to verify the quality of code means flawed tests lead to flawed implementation. But the confidence in flawed implementations are still high since the tests results tell them the code is good.
* From my personal experience: unit tests are sometimes hard to write. For example, there is a private method worth testing but how would a test access it? Reflection will be a solution without changing the original architecture, but it's another complicated thing to both learn and implement. Overall situations like this will require a lot of decision makings and an elegant solution is hard to find.
