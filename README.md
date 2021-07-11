# vscode_snippets
Repository of code snippets for visual studio code

Snippets are a great tool to automate repetitive tasks, and visual studio code allows 
you to use them effectively with the intellisense functionality. But there isn't an 
easy way to save and syncrhonize your vscode snippets across multiple machines, nor
a way to version them. This repository aims at solving all of these issues!


## Use git to manage your vscode snippets
Code snippets in vscode are saved under a plain directory, so we can add a git
repository in it!

To start, copy your existing code snippets to a temporary directory

```
cp /path/to/my/vscode/snippets /path/to/my/vscode/temp_snippets
```

Then delete the `snippets` directory

```
rm -R /path/to/my/vscode/snippets
```

Clone the current directory into the snippets directory

```
git clone git@github.com:louislatreille/vscode_snippets.git /path/to/my/vscode/snippets
```

Copy any of the snippets that you had previously configured into the new `snippets`
directory. Every snippets that you add there will now be versioned with git! Make sure
to commit every now and then ;).