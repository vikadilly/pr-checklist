# pr-checklist
My personal checklist when submitting PRs - based on https://medium.com/swift-india/my-pull-request-review-checklist-to-perform-effective-code-reviews-f4bf2b062e6e
# **General**

 <input type="checkbox" />  Does the code work? Does it perform its intended function, the logic is correct etc.
- [ ]  Is all the code easily understood?
- [ ]  Does it have correct linting?
- [ ]  Is there any redundant or duplicate code?
- [ ]  Is the code as modular as possible?
- [ ]  Can any global variables be replaced?
- [ ]  Can any of the code be replaced with library functions?
- [ ]  Can any logging or debugging code be removed?
- [ ]  Does code follow defined architecture?
- [ ]  Does feature implementation follow UAC and specified design?
- [ ]  Ensure PR passes CI server, re-running once or twice if it fails. Failure could be due to other issues, so determine whether the PR is responsible if failure occurs.
- [ ]  Request changes to the code and/or additional unit tests if any issues are found.
- [ ]  Is any code invoking memory leaks?
- [ ]  Are properties declared with the correct storage semantics? (e.g. weak or unowned instead of strong)
- [ ]  Are good names used for classes, enum, struct , methods, and variables?

# **Documentation or PR explanation**

- [ ]  Is any edge-case handling described?
- [ ]  Is the use and function of third-party libraries documented?
- [ ]  Are data structures and units of measurement explained?

# **Testing**

- [ ]  Is the code testable? i.e. don’t add too many or hide dependencies, unable to initialize objects, test frameworks can use methods etc.
- [ ]  Do tests exist and are they comprehensive? i.e. has at least your agreed on code coverage.
- [ ]  Do unit tests actually test that the code is performing the intended functionality?
- [ ]  Are arrays checked for ‘out-of-bound’ errors?
- [ ]  Could any test code be replaced with the use of an existing API?

# Extras

- [ ]  If using any 3rd party library, check for licenses and compliances
- [ ]  If storing any sensitive information, it must be stored at secure place with encryption technique like HASH STRETCHING or something else.
- [ ]  Avoid Code smells and try to follow Clean Code book concepts by Robert C. Martin.
