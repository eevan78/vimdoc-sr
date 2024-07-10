# Српски превод документације програма Vim 9.1

Архива садржи два директоријума, doc и syntax. У doc директоријуму се налазе
преведени фајлови документације и фајл са ознакама, а у syntax директоријуму
фајл help-sr.vim који садржи додатне дефиниције неопходне за правилно истицање
синтаксе у преведеним фајловима документације.

Да бисте могли користити српски превод документације, директоријуме који се
налазе у архиви најпре морате да распакујете на одговарајуће место.

Препоручујем да их сместите на следећу локацију:

- Windows

  `$HOME\vimfiles` (команда `:echo $HOME` вам исписује вредност променљиве)

- Unix

  `~/.vim`

Програм Vim вам омогућава независан избор језика на којем ће се приказивати
поруке, документација, и менији (у случају да се извршава верзија са графичким
корисничким интерфејсом, gvim).

## Фонт

Да би се текст приказивао како треба, потребно да користите фонт фиксне ширине
који подржава што већи скуп карактера. Као пример, наводим команду коју треба
да поставите у свој _gvimrc фајл када инсталирате бесплатни фонт Iosevka Term
Slab:

```vim
	set guifont=Iosevka_Term_Slab:h14:cEASTEUROPE
```

Постоји доста квалитетних бесплатних фонтова фиксне ширине, а можете да
користите и оне који долазе уз оперативни систем, као што је Consolas на
Windows систему.

За више детаља и примера погледајте документацију.

## Поруке

Ако желите да програм Vim поруке исписује на српском језику, потребно је да
променљиву окружења LANG поставите на одговарајућу вредност.

- Windows

	`LANG=sr_RS@cyrillic`

- Unix
	
  Доста зависи од дистрибуције и љуске коју користите. Употребите излаз
	команде `locale -a` да сазнате вредност на коју треба да поставите
	променљиву LANG. На Ubuntu функционише `LANG=sr_RS.UTF-8`.

## Документација и менији

Кодирање мора бити постављено на utf-8.

Уметните следеће линије на почетак свог vimrc фајла:

```vim
	set encoding = utf-8
	set langmenu = sr " Ако желите српски мени у gvim.
	set helplang = sr " Систем помоћи на српском
```

Излаз команде :version ће вам приказати где се налази vimrc фајл. Вредност
променљивих $VIM и $HOME можете видети помоћу команде echo:
`:echo $VIM`
`:echo $HOME`

Ово је превод стања фајлова документације закључно са закрпом 544 (9.1.544)

## Историја:

- верзија 3.2 (09.07.2024.) - Превод ажуриран на Vim 9.1 ниво закрпе 544
- верзија 3.1 (20.05.2024.) - Превод ажуриран на Vim 9.1 ниво закрпе 414
- верзија 3.0 (15.01.2024.) - Превод ажуриран на Vim 9.1 ниво закрпе 16
- верзија 2.7 (20.09.2023.) - Превод ажуриран на Vim 9.0 ниво закрпе 1898
- верзија 2.6 (18.08.2023.) - Превод ажуриран на Vim 9.0 ниво закрпе 1719
- верзија 2.4 (05.05.2023.) - Превод ажуриран на Vim 9.0 ниво закрпе 1504
- верзија 2.3 (13.02.2023.) - Превод ажуриран на Vim 9.0 ниво закрпе 1294
- верзија 2.2 (30.11.2022.) - Превод ажуриран на Vim 9.0 ниво закрпе 962
- верзија 2.1 (22.09.2022.) - Превод ажуриран на Vim 9.0 ниво закрпе 507
- верзија 2.0 (03.07.2022.) - Превод верзије Vim 9.0
- верзија 1.0 (07.03.2021.) - Урађена је иницијална верзија.
