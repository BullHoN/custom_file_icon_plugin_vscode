# Custom File Plugin Example

It does not use TypeScript and only includes the `vscode` devDependency needed for extension development.

## Documentation link
[Using Custom Language](https://code.visualstudio.com/api/references/contribution-points#contributes.languages)

[Custom Icon Docs](https://code.visualstudio.com/api/extension-guides/file-icon-theme#language-default-icons)


Inside package.json > contributes
```
"languages": [
			{
				"id": "mypackage",
				"extensions": [
					".mypkg"
				],
				"icon": {
					"dark": "./images/custom_icon.svg",
					"light": "./images/custom_icon.svg"
				}
			}
]
```

## Running the Sample

- Run `npm install` in terminal to install dependencies
- Run the `Run Extension` target in the Debug View.

## Create a build

- Run `npm run build` in terminal to create a .vsix build file