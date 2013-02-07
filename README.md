What?
-----

`phpunit` is a command line tool for running 
[PHPUnit](https://github.com/sebastianbergmann/phpunit/) tests. It does not support 
running tests in parallel. `parallel-phpunit` is a command line tool that works the 
same way as `phpunit` but runs the tests in parallel. It searches for PHPUnit tests that
you want to execute, starts multiple `phpunit` commands at the same time to run them, 
monitors and reports the progress and returns the results at the end. The user experience
of `parallel-phpunit` is the same as `phpunit`. In most use cases you can just simply 
replace `phpunit` with `parallel-phpunit` and get the same end result.

Full manual: https://github.com/verkkokauppacom/parallel-phpunit


Changes
----

When using parameter --group run tests only exists selected groups

Why
----
PHPUnit run all providers in test, you can lost more time.