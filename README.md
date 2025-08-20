# Parsing4J
Parsing in Java for INI, JSON, and CSV files!
Extremely simple to use.

## Tutorial:

1. Use the at least Java JRE 9. ☕
2. Download (or build) the .jar file, and then add it to your java classpath.
3. Simply use:
```java
/**
*  Instantiation:
**/
File file = new File("example.json");
Parser p = new Parser(FileType.JSON, file);

/**
*  Parse once:
**/
Tree result = p.parse();

/* Or parse after every change to the file! */
p.parseForChanges(1000L); // Check every 1 second

Tree changingParsedTree = p.getRep(); // You can now get the changed representation on each change

p.disableParsing(); // And turn off the on-changing parser!
```

## Available file formats to parse:

- JSON files (including arrays and sub-objects.
- INI files
- CSV files
- *YAML support coming soon...*

## Other

This project was made by Ra4; it is free use, and contributions are encouraged! Parsing in Java, made easy.
