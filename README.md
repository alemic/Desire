Desire Core staging tree 0.12.2.2

https://www.desire-crypto.com

https://bitcointalk.org/index.php?topic=2272607.0

What is Desire?

Desire is an experimental new digital currency that enables anonymous, instant payments to anyone, anywhere in the world. Desire uses peer-to-peer technology to operate with no central authority: managing transactions and issuing money are carried out collectively by the network. Desire Core is the name of the open source software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of the Desire Core software, see https://bitcointalk.org/index.php?topic=2272607.0.

License

Desire Core is released under the terms of the MIT license. See COPYING for more information or see https://opensource.org/licenses/MIT.

Development Process

The master branch is meant to be stable. Development is normally done in separate branches. Tags are created to indicate new official, stable release versions of Desire Core.

The contribution workflow is described in CONTRIBUTING.md.

Testing

Testing and code review is the bottleneck for development; we get more pull requests than we can review and test on short notice. Please be patient and help out by testing other people's pull requests, and remember this is a security-critical project where any mistake might cost people lots of money.

Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to submit new unit tests for old code. Unit tests can be compiled and run (assuming they weren't disabled in configure) with: make check

There are also regression and integration tests of the RPC interface, written in Python, that are run automatically on the build server. These tests can be run (if the test dependencies are installed) with: qa/pull-tester/rpc-tests.py

The Travis CI system makes sure that every pull request is built for Windows and Linux, OS X, and that unit and sanity tests are automatically run.

Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the code. This is especially important for large or high-risk changes. It is useful to add a test plan to the pull request description if testing the changes is not straightforward.