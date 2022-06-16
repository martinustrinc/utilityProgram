# tokopedia-utility-program

Tokopedia Utility is a utility tool to extracts top 100 product data from Tokopedia with category Mobile Phones/Handphone and store it as CSV file.

It is based on Selenium.

## Requirement
* Java 1.8
* Maven
* [Chrome Driver](https://github.com/SeleniumHQ/selenium/wiki/ChromeDriver)

## Project Build
```mvn clean install```

## JAR Build
```mvn clean compile assembly:single```

Then, JAR file can be found in target directory.

## Run
```java -jar {jar_file} <category> [count]```

Parameter `count` is optional. If not specified, it will be set as 100.

CSV file will be provided with a name in the following format: `Product_<category>_<timeInMillis>.csv`
