# lecture-19-unittests-review

Unit test review

## Run the tests (review)

Unlike last lecture, the tests are in a different directory this time. In
order to run them, tell Python to execute the `unit_tests` module inside `tests/`:

```
vocstartsoft:~/environment $ cd lecture-19-unittests-review/
(for version python 2.7)vocstartsoft:~/environment/lecture-19-unittests-review (master) $ python -m tests/unit_tests
(for version python 3.6)vocstartsoft:~/environment/lecture-19-unittests-review (master) $ python -m tests.unit_tests
.
----------------------------------------------------------------------
Ran 1 test in 0.000s

OK
vocstartsoft:~/workspace/lecture-19-unittests-review (master) $
```

## Write the remaining tests and fix the buggy code! (update!)

Look at function `get_chatbot_response` inside `functions.py`.

It's a buggy function that we partially fixed last lecture. Given a particular
user input, it's intended to return what a chatbot would say.

There are four commands -- `hello`, `add`, `divide`, and `say`, and they should
all be usable like your chatbot would be!

(As an example, `get_chatbot_response("Hey <name>")` should return `"What's up!"`.)

Noticed we fixed the `add` condition of the chatbot and updated our `tests/unit_tests.py` file with a unit test to validate this particular portion of the function. 

Fix the rest of the `get_chatbot_response` function and update the unit tests. 
