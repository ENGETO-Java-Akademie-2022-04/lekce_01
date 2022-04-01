# Cvičení v hodině: Informace o faktuře

Pojďme si nyní společně vyřešit následující cvičení:

1. Vytvořme program, který spočítá celkovou cenu faktury (_invoice price_). Máme zadané:
    - název zboží (_item_), 
    - počet kusů (_number of pieces_),
    - datum vystavení (_date of issue_), 
    - a&nbsp;cenu jednoho kusu (_price per piece_).
    (Další údaje z&nbsp;faktury &mdash; informace o&nbsp;zákazníkovi, datum splatnosti a&nbsp;další nebudeme pro jednoduchost v&nbsp;tomto cvičení řešit.)
2. Přidejme informaci, zda je zákazníkovi poskytnuta sleva (_discount_). Pokud ano, je poslední kus za čtvrtinu původní ceny (ostatní kusy jsou za původní cenu). Upravme kód tak, aby počítal cenu se slevou, pokud byla cena poskytnuta.
3. Vytvoř si metodu pro výpočet celkové ceny faktury (_total price_).
4. Vypiš na obrazovku cenu jednotlivých kusů: vypiš tolik řádků, kolik si zákazník objednal kusů.
5. Přidej ještě jedno zboží. To má jinou cenu a počet kusů.
6. Vytvoř třídu pro uchování jedné položky faktury, abychom údaje o&nbsp;jednom typu zboží spojili dohromady do jednoho objektu.
7. Vytvoř kolekci a&nbsp;přidej do ní obě vytvořené položky faktury.

> Doplnění: 
> 
> 1. Jaké další datové typy v&nbsp;Javě známe?
> 2. Okomentujme také objektové/wrappované číselné typy.
> 3. Odkud budeme brát data? Čtení ze souboru projdeme později.