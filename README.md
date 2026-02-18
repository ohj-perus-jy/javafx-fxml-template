# JavaFX FXML Template Archetype

A Maven archetype for creating a simple, non-modular JavaFX application with FXML.

Designed for beginners, this archetype simplifies the development process by excluding the Java module system.

## Usage

To generate a new project from this archetype, run:

```bash
mvn archetype:generate \
  -DarchetypeGroupId=io.github.ohj-perus-jy \
  -DarchetypeArtifactId=javafx-fxml-template \
  -DarchetypeVersion=1.0.1
```

## Features

- **Non-modular**: No `module-info.java` required, making it easier for beginners.
- **FXML Support**: Pre-configured with a simple FXML layout and controller.
- **IDE Compatible**: Includes a `Main` class to avoid the "JavaFX runtime components are missing" error when running directly from an IDE (like IntelliJ IDEA).
- **Packaging**: Includes configuration for `javafx-maven-plugin` and `jpackage-maven-plugin` to create executable bundles.

## Running the Generated Project

Once the project is generated, you can run it:

1.  **Via Maven**:
    ```bash
    mvn javafx:run
    ```
2.  **Via IDE**:
    Run the `main` method in the `Main` class.

## Build and Install Locally

If you want to build this archetype from source:

1.  Install the archetype to your local repository:
    ```bash
    mvn install
    ```
2.  Generate a project using the local catalog:
    ```bash
    mvn archetype:generate -DarchetypeCatalog=local
    ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

This project was forked from [sosuisen/jfx-sss-fxml](https://github.com/sosuisen/jfx-sss-fxml).
