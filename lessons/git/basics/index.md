nebo dokonce kolegům, kteří na ni spolupracují.
> [note]
> Budeme hodně pracovat s příkazovou řádkou.
> Jestli se s ní ještě nekamarádíš, koukni se na
> [úvod]({{ lesson_url('beginners/cmdline') }}).
> 
> Nezapomeň: `$` na začátku se nepíše;
> je tu proto, aby šlo poznat že jde o příkaz.
Na první pohled to vypadá, že se nic nestalo.
Pak soubor ulož a zavři editor.

> [note] Jak na editory?
>
> Na Windows, máš-li
> [správně nastavený Git]({{ lesson_url('git/install') }}),
> se použije Poznámkový blok (Notepad) – stačí něco
> napsat, uložit (<kbd>Ctrl</kbd>+<kbd>S</kbd>) a zavřít
> (<kbd>Alt</kbd>+<kbd>F4</kbd>).
>
> Na Linuxu a macOS se objeví editor v příkazové řádce,
> který se jmenuje Nano.
> Pozná se tak, že v dolních dvou řádcích má malou nápovědu.
> Něco napiš, pomocí <kbd>Ctrl</kbd>+<kbd>O</kbd>
> soubor ulož, potvrď jméno souboru (<kbd>Enter</kbd>)
> a pomocí <kbd>Ctrl</kbd>+<kbd>X</kbd> editor zavři.
>
> Nemáš-li Git nastavený podle instrukcí, objeví se přímo
> v příkazové řádce Vim – poměrně složitý editor, který
> se teď učit nebudeme. Pozná se tak, že úplně
> spodní řádek je prázdný.
> V takovém případě stiskni
> <kbd>Esc</kbd>, napiš `:q!` (dvojtečka, Q, vykřičník)
> a potvrď pomocí <kbd>Enter</kbd>.
> Pak si nastav Git a zkus `git commit` znovu.
popisek
> [note]
> Když je výpis moc dlouhý, můžeš se v něm pohybovat
> (<kbd>↓</kbd>, <kbd>↑</kbd>, <kbd>PgUp</kbd>, <kbd>PgDn</kbd>)
> a zpět se dostaneš klávesou <kbd>Q</kbd> jako *Quit*.

> [note] Kódování ve Windows
> Pokud výpis nezvládá znaky s diakritikou, zadej před  `git show` příkaz
>
> ```dosvenv
> > set LC_ALL=C.UTF-8
> ```
>
> Tento příkaz nastaví aktuální terminál: když si ovevřeš nové okno
> s příkazovou řádkou, bude ho potřeba zadat znovu.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
        ␛[31mmodified:   basnicka.txt␛[m
no changes added to commit (use "git add" and/or "git commit -a")
> [note]
> Změnilo-li se na řádku jen jedno slovo nebo i písmeno,
> celý řádek se ukáže jako smazaný a zase přidaný.
> Dá se to nastavit i jinak, když je potřeba,
> ale je dobré si na tento standard zvyknout.
> [note]
> Řádek začínající <tt class="blue">@@</tt> říká,
> kde v souboru změna je (u mě začínal vypsaný kousek
> souboru řádkem 1 a měl 6 řádků; v nové verzi je
> opět od 1. řádku, ale narostl na 9).
Jsi-li se změnami spokojen{{a}}, řekni Gitu, ať je
A pro úplnost se znovu koukni, co říká
následuje prázdný řádek a pak detailnější popis důvodů
Nemá cenu popisovat, co je jasné ze změn samotných,
Cokoli, co může přijít vhod, až se změny bude snažit někdo pochopit.
takhle se to líp čte. (Ale co si budeme povídat, hlavní 
důvod je ukázat, co dělá git diff.)
> [note]
> Nebude-li se ti někdy dařit shrnout změnu
> v 70 znacích, zamysli se, jestli neděláš moc velkou
> změnu najednou – např. "změna řetězce X
> a dopsání nového cyklu Y" by bylo lepší uložit
> jako dvě různé revize.
    takhle se to líp čte. (Ale co si budeme povídat, hlavní
    důvod je ukázat, co dělá git diff.)
    takhle se to líp čte. (Ale co si budeme povídat, hlavní
    důvod je ukázat, co dělá git diff.)
Git log vypíše všechny revize od té nejnovější až po
Až budeš mít verzí tolik, že se nevejdou najednou
> [note]
> Je spousta možností jak vypisovat historii pomocí `git log`.
> Všechno je podrobně – možná až moc podrobně –
> popsáno v dokumentaci; stačí zadat `git help log`.
> „Ven“ z dokumentace se opět dostaneš klávesou <kbd>q</kbd>.
>
> Já často používám `git log --oneline --graph --decorate --cherry-mark --boundary`.
> Chceš-li tyhle možnosti studovat, začni v tomto
> pořadí a dej si pauzu vždycky, když přestaneš
> rozumět. :)
psali programátoři, které místo designu zajímá, co je
udělej dalších pár revizí a koukni se na ně přes
aktuální verze souborů se uloží a už nejde (jednoduše)
Jednotlivé verze a změny od posledního uložení,
Takže odteď, kdykoliv uděláš v rámci PyLadies funkční