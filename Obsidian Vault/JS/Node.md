
- open source
- Cross-platform - windows, Linux, macOS
- JavaScript runtime environment - A runtime environment is like a virtual machine that executes code
- Web applications: Node.js is often used to build both front-end and back-end components
- single process, without creating a new thread for every request
- Asynchronous I/O Primitives
- Non-Blocking Behavior
- In Node.js the new [[ECMAScript]] standards can be used without problems

### Express

- ## installing express
	- create directory
	- npm init
	- npm install express
- ## set-up node js server
	- write endpoint
	- initialize instance
	- run server
- ## express generator
	- application generator tool, `express-generator`, to quickly create an application skeleton
	- NPX stands for **Node Package eXecute**. It is simply an NPM package runner. It allows developers to execute any Javascript Package available on the NPM registry without even installing it
	- NPX is installed automatically with NPM version 5.2.0 and above
- ## basic routing
	- ```javascript
	app.METHOD(PATH, HANDLER)
	
	Where:
	
	- `app` is an instance of `express`.
	- `METHOD` is an http method
	- `PATH` is a path on the server.
	- `HANDLER` is the function executed when the route is matched.```
	- app.get
	- res.send()
- ## serving static files
	- 