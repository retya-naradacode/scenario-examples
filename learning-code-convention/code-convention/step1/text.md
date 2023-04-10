
Code Convention Using Super Linter

The GitHub Super Linter was built out of necessity by the GitHub Services DevOps Engineering team to maintain consistency in our documentation and code while making communication and collaboration across the company a more productive experience. 

<br>

### Solution

The Super Linter solves many of these requirements through automation. Some included features:

Prevent broken code from being uploaded to master branches
Help establish coding best practices across multiple languages
Build guidelines for code layout and format
Automate the process to help streamline code reviews
With these basic criteria, we should be shipping better, cleaner, and more stable code internally and to our customers and partners



```plain
Super Linter Docker Images

docker pull github/super-linter:slim-v4
```

Try to lint Repository

```plain
Git Repository

https://gitlab.com/apitestingnarada/springboot-practice.git
```

Standardizing a rule set across the Super Linter has been an interesting challenge as each developer is unique in how they code. This is why we allow users to use any rules for the linter as they see fit for their repository. But, if no ruleset is defined, we must default to a certain standard.

References :
https://github.com/github/super-linter






