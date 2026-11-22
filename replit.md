# Student records console program

This project is a Java console application. It keeps student records in `db.txt`;
it does not serve a website or require secrets or external services.

## Run on Replit

Use the **Run** button and read the output in **Console**. The `Start application`
workflow compiles the three Java source files and runs `Main`:

```sh
javac -d . src/main/java/Main.java src/main/java/Service.java src/main/java/Student.java && java -cp . Main
```

The program prints the saved students and exits normally. Each run appends
Krzysztof (20) and Janusz (40) to `db.txt`, so repeated runs create duplicate
records. This is the original program behavior.

## Environment

The Replit Java module supplies the JDK and Java tooling. `replit.nix` deliberately
has no extra dependencies; do not duplicate the Java module's tools there.
The application itself uses only the Java standard library. The imported Maven
file includes JUnit, but Maven dependencies are not needed for this run command.

Keep the current source layout under `src/main/java/`.
