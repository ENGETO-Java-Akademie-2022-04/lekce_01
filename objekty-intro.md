# Objekty &mdash; spojme data a&nbsp;metody

Co kdybychom chtěli počítat vlastnosti obdélníků, kruhů a&nbsp;trojúhelníků.

Mít všechny proměnné a&nbsp;metody pohromadě by bylo nepřehledné. Můžeme tedy spojit proměnné (atributy) a&nbsp;odpovídající metody a&nbsp;vytvoříme _třídu_.

V&nbsp;Javě takto existují například třídy:

* `Integer`
* `Double`
* `BigDecimal` (vhodné například pro práci s&nbsp;peněžními částkami)
* `Boolean`
* `Char`

Tyto třídy zahrnují kromě samotné hodnoty i&nbsp;metody, které se k&nbsp;datovým typům vztahují. Například:

```java
        String input = "0";
        // ... kód, který načte hodnotu input ze souboru ...
        int length = Integer.parseInt(input); 
        // převede text na číslo

        LocalDate today = LocalDate.now();
```

Třídami jsou také:
- `String` (textový řetězec)
- `LocalDate` (datum)

## Vlastní objekty

```java
package com.engeto.example;

public class Rectangle {
    /*
        * Properties of rectangle
        */
    private double base; // základna
    private double height; // výška

    public Rectangle(double base, double height) {
        this.base = base;
        this.height = height;
    }

    public double perimeter() {
        return (base + height) * 2;
    }

    public double area() {
        return base * height;
    }

    public double diagonalLength() {
        return Math.sqrt( Math.pow(base,2) + Math.pow(height,2) );
    }
}
```

> Ale třídy si budeme muset vysvětlit podrobněji &mdash; to už si necháme na příště... ;) :D


--- 

[Zpět na obsah lekce...](README.md)
