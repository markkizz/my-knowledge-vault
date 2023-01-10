Data platform
- [node-sql-parser - npm (npmjs.com)](https://www.npmjs.com/package/node-sql-parser)
- [koca/vue-prism-editor: A dead simple code editor with syntax highlighting and line numbers. 3kb/gz (github.com)](https://github.com/koca/vue-prism-editor)
- data model
	- repositories/$uuid
```ts
interface Repositories {
	id: string
	name: string
	userId: string
	sourceCode: string // or node-sql-parse type
	language: string // can be more than SQL 
	tags: {
		[tagName: string]: boolean
	}
}

interface Tag {
	id: "name"
	name: string //uniq
}
```
	 - 