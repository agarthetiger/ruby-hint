# ruby-hint

Hint CLI tool rewritten in Ruby. 'hint' started off as a python project to help me learn python, with the benefit that the output was a useful-to-me tool to get my personal hints directly on the command line. I'm working with a predominantly Ruby development team at the moment so I'm re-writing this tool in Ruby as an exercise in learning Ruby, also with the benefit of being a real project rather than a set of theoretical coding exercises.

## Run me

If your file is executable, the shebang at the top tells the system what to run it with, so you can run like a command.

```bash
./hint
```

I might want to look at using an executable in a /bin folder in a redistributable gem to make the exe run as a command available in the path from anywhere. More investigation required into how to bundle and distribute a Ruby-based executable.

## Edit me

Ruby and Git - https://rubydoc.info/gems/git/Git.html

## Test me

If I keep most of the functionality as Plain Old Ruby Objects the code should be more testable, and looser coupled to any CLI framework.

Currently there are no tests.

## CLI

The mechanics of a cli are not key for me, so I'll try https://dry-rb.org/gems/dry-cli/0.6/ and see how this works. Also used is the Thor gem used by Rails. Unfortunately neither of these support the bare command with parameters and I'm not gaining much by using either of these. argv and optparse are probably sufficient for my needs here.
