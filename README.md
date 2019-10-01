# lecture-19-unittests-review

Unit test review

## Run the tests

Unlike last lecture, the tests are in a different directory this time. In
order to run them, tell Python to execute the `unit_tests` module inside `tests/`:

```
vocstartsoft:~/environment $ cd lecture-19-unittests-review/
vocstartsoft:~/environment/lecture-19-unittests-review (master) $ python -m tests/unit_tests
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
vocstartsoft:~/workspace/lecture-19-unittests-review (master) $
```

## Write more tests and fix the buggy code!

Look at function `get_chatbot_response` inside `functions.py`.

It's a buggy function that I slapped together real quick. Given a particular
user input, it's intended to return what a chatbot would say.

There are four commands -- `hello`, `add`, `divide`, and `say`, and they should
all be usable like your chatbot would be!

(As an example, `get_chatbot_response('Hello')` should return `'Hey there!'`.)

Modify `tests/unit_tests.py` and write and run some unit tests that
codify expected input/output combinations for this function.

As you write and run the tests, you'll find bugs in the code. Fix them and
write tests for your fixes :)

## Finished?

Get a head start with continuous integraton. Read the following article:
* https://www.martinfowler.com/articles/continuousIntegration.html
