# Metody

Zatím jsme si pojmenovali hodnoty tím, že jsme je uložili do proměnných. Výhoda je, že proměnnou mohu používat opakovaně.

Co když chci ale opakovaně provádět stejný výpočet? Třeba chci počítat délku úhlopříčky různých obdélníků. Můžeme si proto připravit _metodu_, která bude výpočet popisovat:

```java
package com.engeto.example;

public class Main {

    public static double diagonalLength(double base, double height) {
        return Math.sqrt( Math.pow(base,2) + Math.pow(height,2) );
    }

    public static void main(String[] args) {
        /*
         * Properties of rectangle
         */
        double base = 5; // základna
        double height = 7; // výška
        // Obvod:
        double perimeter = (base + height) * 2;
        System.out.println("Perimeter: "+perimeter);
        double baseHeightRatio = base/height;
        System.out.println("Base/height ratio: "+baseHeightRatio);
        double area = base*height;
        System.out.println("Area: "+area);
        double diagonal = diagonalLength(base, height);
        System.out.println("Diagonal length ("+base+","+height+"): "+diagonal);
        base = 10; height = 2;
        diagonal = diagonalLength(base, height);
        System.out.println("Diagonal length ("+base+","+height+"): "+diagonal);
    }
}
```

## Modifikátory
Při deklaraci metod můžeme použít některá klíčová slova:

- <b>static</b> - tohle klíčové slovo říká, že proměnná má existovat po celou dobu běhu programu &mdash; lépe pochopíme, až si ukážeme objekty.

- <b>public</b>, <b>protected</b>, <b>private</b> - tato klíčová slova definují viditelnost proměnné z&nbsp;jiných objektů.

--- 

[Zpět na obsah lekce...](README.md)
