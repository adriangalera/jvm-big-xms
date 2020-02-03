# jvm-big-xms

## Generate the jar

```
./gradlew jar
```

## Experiments

Running with 2G of Xms:
```
java -Xms 2G -jar build/libs/boom-1.0-SNAPSHOT.jar
```
Running with 100G of Xms:
```
java -Xms100g -jar build/libs/boom-1.0-SNAPSHOT.jar 
```
Pre reserve the Xms memory:
```
java -XX:+AlwaysPreTouch -Xms100g -jar build/libs/boom-1.0-SNAPSHOT.jar 
```