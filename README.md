# Groundhog

A simple pure Java tool to crawl software development projects from popular forges and to extract metrics from them.

## Usage

Groundhog uses Java 7 features, so you must have it installed before build.

### Building in your machine

Groundhog was built using Maven. In order for it to behave like an Eclipse project, you'll need to install [1] Maven, and then run:

```
$ mvn eclipse:eclipse
```

### Generating the JAR

Generate the JAR file for the Groundhog project.

```
$ mvn package
```

Eclipse users can go to `File > Export > Runnable Jar File` and enter the `CmdMain` class for the option "Launch Configuration".

### Running Groundhog

Search GitHub for projects matching "phonegap-facebook-plugin" and place the results (if any) in a folder called metrics:

```shell
$ java -jar groundhog.jar -forge github -out metrics phonegap-facebook-plugin
```

## Info

### Supported Forges

* GitHub
* Google Code
* SourceForge

### Crawlers

### Supported Programming Languages

* Java, parsing only (more to be added later)

### Forge Search

* **GitHub**:
Groundhog uses the [GitHub API v3] to search for repositories on GitHub

* **Google Code**:
to be written

* **SourceForge**:
to be written

## Documentation

Groundhog features a [Wiki], where you can browse for more information.

You can generate the Javadoc files with the following command:

```
$ cd src/
$ javadoc -d src/src/groundhog br.cin.ufpe.groundhog
```

## Core team

* Flávio Junior {fjsj@cin.ufpe.br}

* Gustavo Pinto {ghlp@cin.ufpe.br}

* Rodrigo Alves Vieira {rav2@cin.ufpe.br}

* Danilo Neves Ribeiro {dnr2@cin.ufpe.br}
 
* Fernando Castor {myfamilyname@cin.ufpe.br}

## How to contribute

Want to contribute with code, documentation or bug report?

Just add an issue and fix them! :)
Try the [existing ones](https://github.com/spgroup/groundhog/issues)

## License

Groundhog is released under GPL 2.

[1]: Consider installing the [m2e] plugin for Eclipse

[GitHub API v3]: http://developer.github.com/
[m2e]: http://eclipse.org/m2e/
[Wiki]: https://github.com/spgroup/groundhog/wiki
=======
