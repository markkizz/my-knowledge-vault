Data platform
- [node-sql-parser - npm (npmjs.com)](https://www.npmjs.com/package/node-sql-parser)
- [koca/vue-prism-editor: A dead simple code editor with syntax highlighting and line numbers. 3kb/gz (github.com)](https://github.com/koca/vue-prism-editor)
- data model
	- user/repositories
	- repositories/project
```ts
interface Repositories {
	id: string
	name: string
	userId: string
	member?: Array<string>
}

interface Project {
	id: string
	name: string
	userId: string
	sourceCode: string // or node-sql-parse type
	language: string // can be more than SQL 
	tags: {
		[tagName: string]: boolean
	}
	repository: string
	/* table: {
		[tableName: string]: boolean
	}
	*/
}

interface Tag {
	id: string // tag name uniq
	name: string
}
```
	 - 