# JavaScript Await forEach

Asynchronous forEach function. To let you await for the forEach.

## Getting Started

Install with nodeJS.

```console
npm install await-for-each
```

## How to use

```javascript
// Import the module
import forEach from 'await-for-each';

// You need to use it inside a async function to be able to wait for it to be finish
async run () {
	// Setting up a array to iterate
	const array = [0, 1, 2, 3];

	// Wait for the forEach to iterate the array
	await forEach(array, async (value, index) => {

		// Feel free to wait for anything here
		await something(value);
	});

	// The iteration is finish
	console.log('Finish');
}

// Kick off
run();
```

## License

Copyright (c) 2018 "Beckan" Daniel Bäckström  
Licensed under the MIT license.