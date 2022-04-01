
# První projekt

Postup pro vytvoření prvního projektu si ukážeme společně. Stručně:
1. Po spuštění IDEI klikneme na "New project" 
2. zvolíme Java project
3. použijeme šablonu "Console app"
4. zadáme jméno projektu
5. a&nbsp;máme vytvořený náš první projekt.

> Můžete využít [návod ve studijních materiálech](https://engeto.com/cs/kurz/java-1-uvod-do-programovani/studium/OFMSGkbhQJSmt5iHBNwUuQ/zaciname-s-javou/tvuj-prvni-projekt/program-hello-world).

## Hello World!

Pakliže Java není Váš první programovací jazyk, tak jistě tušíte, co si představit pod "Hello, world!". Pokud ne, tak vězte, že je jde o program používaný k testování toho, že máme vše potřebné pro vývoj v tom kterém programovacím jazyce, který nedělá nic víc, že někam vypíše větu "Hello, world!" - od toho pochází i jeho název (tradičně jde o&nbsp;první psaný a spouštěný program, když se učíte nový jazyk).

K tomu, abychom ho zvládli napsat, budeme potřebovat metodu pro výpis v textu - `System.out.println(<i>sem přijde to, co chceme vypsat</i>)`.

## Třída `Main` a metoda `main`

V našem projektu bude jedna třída pojmenovaná Main a v ní metoda pojmenovaná main:

```java
package com.engeto.example;

public class Main {

    public static void main(String[] args) {
	// write your code here
    }
}
```
Jak komentář napovídá a jak jsme si už řekli, metoda `main` je vstupní bránou do našeho programu &mdash; tato metoda je tou, co se spustí, když spustíme náš program a z&nbsp;ní voláme všechny ostatní metody, případně kód píšeme přímo do ní.

Jak jsme si řekli, tak metoda `System.out.println` slouží pro výpis textu a už i víme, kam ji umístit, aby se provedla - do metody `main` - do závorek jí jako parametr předáme to, co chceme vypsat, což je v našem případě text "Hello, world!". Výsledný kód pak bude vypadat takto:

```java
package com.engeto.example;

public class Main {

    public static void main(String[] args) {
	      System.out.println("Hello, world!");
    }
}
```

## Balíčky

Balíček v Javě představuje skupinu souvisejících tříd. Jde si ho představit jako souborový systém kdy balíčkem je složka - která může mít podbalíčky - podsložky a jednotlivé třídy, rozhraní a enumy jsou pak soubory.

To, do jakého balíčku naše třída/enum/interface patří, specifikujeme pomocí klíčového slova package, za kterým následuje cesta k té náší X.

Pokud bychom měli třídu Ruler v podbalíčku utilities uvnitř balíčku geometry, tak by zápis vypadal takto:

```java
package geometry.utilities;

public class Ruler {

}
```

## Aritmetické operátory

Počítač je nástroj pro počítání. Pojďme vyzkoušet, jesti jde v&nbsp;Javě spočítat, kolik je 5 plus 7.


```java
package com.engeto.example;

public class Main {

    public static void main(String[] args) {
	      System.out.println(5+7);
    }
}
```

Co ostatní aritmetické operátory?

Operace | Zápis v Javě
---- | :----:
 sčítání | +
 odčítání | -
 násobení | *
 dělení | /
 zbytek po dělení | %
 zvyš o 1 | ++
 sniž o 1 | --
 mocnina | Math.power(x, y)
 druhá odmocnina | Math.sqrt(x)

 Více viz: [Java#1 Základní operace](https://learn.engeto.com/cs/kurz/java-1-uvod-do-programovani/studium/oLTq9_cOTgyRFzmGy4alFg/popis-vypoctu-operatory-podminky-cykly-a-debugovani/zakladni-operace/ciselne-typy-a-operace-s-nimi)


```java
package com.engeto.example;

public class Main {

    public static void main(String[] args) {
        System.out.println((5+7)*2);
        System.out.println(5/7);
        System.out.println(5*7);
        System.out.println(Math.sqrt( Math.pow(5,2) + Math.pow(7,2) ));
    }
}
```

> Jenže kdo pochopí, co to tady vlastně počítám???

## Komentáře v kódu

Kód můžeme zpřehlednit tak, že doplníme komentáře:

Typ komentáře | Zápis v Javě
----- | -----
Do konce řádku | `// Komentář`
Blok - i přes více řádků | `/* Komentář */`
Dokumentace | `/** Komentář */`

Pomocí komentářů bychom mohli vysvětlit, že se jedná o výpočet parametrů obdélníku.

> Jenže &mdash; co když někdo zapomene upravit komentáře a&nbsp;kód změní???
>
> To bys samozřejmě nikdy neudělal(a), ale udržování komentářů stojí čas. Bylo by lepší pojmenovat jednotlivé hodnoty a kód zpřehlednit &rarr; jdeme na proměnné! 

--- 

[Zpět na obsah lekce...](README.md)
