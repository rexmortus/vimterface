# Vimterface

Vimterface is a vim-like user interface for web applications, written in Javascript.

It is inspired by projects like [vimperator](http://www.vimperator.org/) which add modal, vim-like functionality to applications that are not text editors.

The notion is simple. Vimterface adds a UI component into the DOM and allows you to bind keystrokes to user-defined functions. It also has a command mode.

## Example usage

```
vimterface.init()
```

Calling `vimterface.init()` loads the vimterface UI into the DOM.

Add keystroke bindings with `vimterface.bind()`, for example:

```
vimterface.bind('k', function(){
	scrollBy();
})
``` 

Add commands with `vimterface.command()`, for example:

```
vimterface.command('project', function(args){
	doStuff();
})
```
Entering command mode gives you a full, auto-completeable list of registered commands.

