# Commit Style Guidelines for Kiwix-Android

### How to Write Good Commit Messages

A commit message consists of 3 parts:
- shortlog
- commit body
- issue reference

Example:
```
setup.py: Change filename Setup --> setup

The file name was misleading.

Closes https://github.com/oss2019/information-security/issues/5861
```

Shortlog
Example:
```
Change filename Setup --> setup
```
- Maximum of 50 characters.(Keeping subject lines at this length ensures that they are readable, and explains the change in a concise way.)
- Should describe the change - the action being done in the commit.
- Should not include WIP prefix.
- Should have a tag and a short description separated by a colon (:)

Commit Body
Example:
```
The file name was misleading.
```

- Maximum of 72 chars excluding newline for each line.(The recommendation is to add a line break at 72 characters, so that Git has plenty of room to indent text while still keeping everything under 80 characters overall.)
- Not mandatory - but helps explain what you’re doing.
- Should describe the reasoning for your changes. This is especially important for complex changes that are not self explanatory. This is also the right place to write about related bugs.
- First person should not be used here.

Issue reference
Example:

```
Closes https://github.com/oss2019/information-security/issues/5861
```

- Should use the `Fixes` keyword if your commit fixes a bug, or `Closes` if it adds a feature/enhancement.
- In some situations, e.g. bugs overcome in documents, the difference between `Fixes` and `Closes` may be very small and subjective. If a specific issue may lead to an unintended behaviour from the user or from the program it should be considered a bug, and should be addresed with `Fixes`. If an issue is labelled with `type/bug` you should always use `Fixes`
- Should use full URL to the issue.
- There should be a single space between the `Fixes` or `Closes` and the URL.

A full documented guide can be found at [api.coala.io](http://api.coala.io/en/latest/Developers/Writing_Good_Commits.html).
### Title
The title consists of the subject and type of the commit message.

### Type
The type is contained within the title and can be one of the following types:

* **Implement** feature x
* **Fix** a bug in x feature
* **Improve** documentation for x feature
* **Remove** removed redundant code
* **Restyle** formatting, missing semi-colons, etc; no code change
* **Refactor** refactoring production code

### Subject
The subject is a single short line summarising the change. It should be no greater than 50 characters, should begin with a capital letter and do not end with a period.

Use an imperative tone to describe what a commit does, rather than what it did. For example, use fix; not fixed or fixes or fixing.

For example:
- Fix typo in Commit Style guidelines
- Add crash reporting via e-mail
- Implement SearchActivity using MVP pattern

Instead of writing the following:
- Fixed bug with Y
- Changing behaviour of X

### Body
The body includes the kind of information commit message (if any) should contain.

Not every commit requires both a subject and a body. Sometimes a single line is fine, especially when the change is self-explanatory and no further context is necessary, therefore it is optional. The body is used to explain the what and why of a commit, not the how.

When writing a body, the blank line between the title and the body is required and we should try to limit the length of each line to no more than 72 characters.

***
