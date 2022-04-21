# subcommand
Modern command-line applications often implement “sub-commands” to bundle a suite of tools under a single command. The most well-known tool that uses this pattern is git. When examining a command like git init, git is the command and init is the sub-command of git. One notable feature of sub-commands is that each sub-command can have its own collection of flags.  Go applications can support sub-commands with their own set of flags using the flag.(*FlagSet) type. To illustrate this, create a program that implements a command using two sub-commands with different flags.

This example illustrates some principles behind how larger command line applications could be structured in Go. FlagSets are designed to give developers more control over where and how flags are processed by the flag parsing logic.

link:
https://www.digitalocean.com/community/tutorials/how-to-use-the-flag-package-in-go