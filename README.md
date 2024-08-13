GO + AIR + HTMX + TAILWIND

## 👨‍🚀 Setup:

Besides the obvious prerequisite of having Go! on your machine, you must have Air installed for hot reloading when editing code.

Start the app in development mode:

```
$ air # This also compiles the view templates automatically / Ctrl + C to stop the application
```

Build for production (previously it is necessary to regenerate the templates with the `templ generate` command; see explanation below):

```
$ go build -ldflags="-s -w" -o ./bin/main . # ./bin/main to run the application / Ctrl + C to stop the application
```

>[!TIP]
>***In order to have autocompletion and syntax highlighting in VS Code for the Teml templating language, you will have to install the [templ-vscode](https://marketplace.visualstudio.com/items?itemName=a-h.templ) extension (for vim/nvim install this [plugin](https://github.com/joerdav/templ.vim)). To generate the Go code corresponding to these templates you will have to install the templ CLI:***

```
$ go install github.com/a-h/templ/cmd/templ@latest
```

>[!TIP]
>***And then regenerate the templates with the command:***

```
$ templ generate # The `templ generate --watch` command will watch the project folder to regenerate them every time we make a change to its code.
```

>[!TIP]
>***Review the documentation on Templ [installation](https://templ.guide/quick-start/installation) and [support](https://templ.guide/commands-and-tools/ide-support/) for your IDE.***

---

### Happy coding 😀!!
