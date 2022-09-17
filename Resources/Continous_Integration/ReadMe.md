## Continuous integration

### Makefile:

Makefile is a good alternative to a bunch of bash scripts used to automate tedious tasks. It tracks files’ dependency graph, and “last modified” timestamps of the files. If one of dependencies timestamp is greater than the one of the original file, the original file needs to be rebuilt.


### Linters:

Linters analyze code to detect various categories of lint. Those categories can be broadly defined as the following:

- Logical Lint
	- Code errors
	- Code with potentially unintended results
	- Dangerous code patterns
- Stylistic Lint
	- Code not conforming to defined conventions


|Linter|	Category	|Description|
|---|---|---|
|Pylint	|Logical & Stylistic	|Checks for errors, tries to enforce a coding standard, looks for code smells|
|PyFlakes	|Logical	|Analyzes programs and detects various errors|
|pycodestyle	|Stylistic	|Checks against some of the style conventions in PEP 8|
|pydocstyle	|Stylistic	|Checks compliance with Python docstring conventions|
|Bandit	|Logical	|Analyzes code to find common security issues|
|MyPy	|Logical	|Checks for optionally-enforced static types|

|Tool	|Category	|Description|
|---|---|---|
|Mccabe	|Analytical	|Checks McCabe complexity|
|Radon	|Analytical	|Analyzes code for various metrics (lines of code, complexity, and so on)|
|Black	|Formatter	|Formats Python code without compromise|
|Isort	|Formatter	|Formats imports by sorting alphabetically and separating into sections|

### GitHub Actions

- SaaS-based build server
- Allows you to do Continous Integration.
- YAML-based high level and simple configuration file.