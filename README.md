## Introduction
Client of zhuque - a log collecting and analysing platform. visite https://github.com/azl397985856/zhuque for more info

## Usage
copy zhuque-client.js into your workspace and import it by injecting script tag

```js
// for error log
errorLog.init({
	  remoteLogging: true,
	  remoteSettings: {
	    url: 'http://localhost:1333/log',
	    additionalParams: {
	      userId: '1089288',
	      username: 'zpl',
	      password: 'zpl',
	      type: 'error'
	    },
	    successCallback: function () {
	      console.log('errorLog logged.');
	    },
	    errorCallback: function () {
	      console.log('Err! Something went wrong.');
	    }
	  }
});
// for performance log
perfLog.init({
  remoteLogging: true,
  remoteSettings: {
    url: 'http://localhost:1333/log',
    additionalParams: {
      userId: '1089288',
      username: 'zpl',
      password: 'zpl',
      type: 'performance'
    },
    successCallback: function () {
      console.log('perfLog logged.');
    },
    errorCallback: function () {
      console.log('Err! Something went wrong.');
    }
  }
});
```

## Contribution

We welcome all contributions, please submit any ideas as [pull requests](https://github.com/azl397985856/zhuque/pulls) or as a [GitHub issue](https://github.com/azl397985856/zhuque/issues).
## Licence
MIT
