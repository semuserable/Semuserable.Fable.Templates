# What's inside

Fable minimal templates with the most recent versions of `npm` and `dotnet` libraries. Each template contains `README.md` with instructions, but usually it's just a simple `npm install && dotnet build && npm start`.

- `fable-empty` contains `Fable` without `React` or `Elmish`
	- `npm` libs
		- [@babel/core](https://www.npmjs.com/package/@babel/core)
		- [fable-compiler](https://www.npmjs.com/package/fable-compiler)
		- [fable-loader](https://www.npmjs.com/package/fable-loader)
		- [webpack](https://www.npmjs.com/package/webpack)
		- [webpack-cli](https://www.npmjs.com/package/webpack-cli)
		- [webpack-dev-server](https://www.npmjs.com/package/webpack-dev-server)
    - `dotnet` libs
      - [Fable.Core](https://github.com/fable-compiler/Fable/tree/master/src/Fable.Core)
- `fable-react` contains `React` bindings for `Fable` with several examples without `Elmish`
	- `npm` libs
		- [@babel/core](https://www.npmjs.com/package/@babel/core)
		- [fable-compiler](https://www.npmjs.com/package/fable-compiler)
		- [fable-loader](https://www.npmjs.com/package/fable-loader)
		- [react](https://www.npmjs.com/package/react)
		- [react-dom](https://www.npmjs.com/package/react-dom)
		- [webpack](https://www.npmjs.com/package/webpack)
		- [webpack-cli](https://www.npmjs.com/package/webpack-cli)
		- [webpack-dev-server](https://www.npmjs.com/package/webpack-dev-server)
    - `dotnet` libs
      - [Fable.Core](https://github.com/fable-compiler/Fable/tree/master/src/Fable.Core)
      - [Fable.React](https://github.com/fable-compiler/fable-react)

# How to use

* install templates

```code
dotnet new -i Semuserable.Fable.Templates::1.0.0
```

* use templates

```code
dotnet new fable-empty
dotnet new fable-react
```

* uninstall templates

```code
dotnet new -u Semuserable.Fable.Templates
```

# How to create

All templates are located in `templates` folder. Create new folder and put new template there. Use the existing ones as an example.

* edit `templatepack.csproj` to change package details
* create a package
```
dotnet pack
```
* new package will be in `bin/debug` folder (ex. `Semuserable.Fable.Templates.1.0.0.nupkg`)