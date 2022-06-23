# How to add custom metadata to automation tests in UnitTest on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=UnitTest-custom-metadata)

If you want to add custom metadata to automation tests in UnitTest on LambdaTest, you can follow the steps below. You can refer to sample test repo [here](https://github.com/LambdaTest/Python-UnitTest-Selenium).

# Steps
With LambdaTest, you can add custom meta data to automation tests. These are added for tests by setting the data in `customData` capability. The code below illustrates the usage:

```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "customData": [ 	
						{ "_id": "5f46aaa69adf77cfe2bb4fd6", 
						"index": "0", 
						"guid": "9451b204-12f0-4177-8fe9-fb019b3e4bf3", 
						"isActive": "False", 
						"picture": "http//placehold.it/32x32" } ]  
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```


## Run your test

```bash
python lambdatest_test.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

