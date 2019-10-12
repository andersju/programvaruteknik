---
title: Programvaruteknik
---
## Innehållsförteckning
{:.no_toc}

* TOC
{:toc}

## Inledande tips

* Se till att vidarebefordra din studentmejl till din vanliga mejl, så att du inte missar något viktigt! Logga in med dittanvändarnamn@student.miun.se på <https://mail.google.com/> och ändra i inställningarna.
* Gå med i [Programvaruteknik på Discord](https://discordapp.com/invite/FTCnyDf) (OBS: endast för studenter)

## Kurslitteratur

### Elektroniskt

Biblioteket som har ungefär allt: Library Genesis (googla).

Är LibGen blockerad? Byt till en DNS-server som inte tvingats ljuga för dig, så kommer det förmodligen att fungera. Det finns [många öppna sådana](https://en.wikipedia.org/wiki/Public_recursive_name_server). De som tillhandahålls av Google (8.8.8.8 och 8.8.4.4) och Cloudflare (1.1.1.1) har lättihågkomliga IP-adresser.

### Döda träd

Lån, campusstudenter: [universitetsbiblioteket](https://biblioteket.miun.se/)

Lån, student ej i Östersund men i Sverige: [KB:s tjänst Libris](http://libris.kb.se/) vet vad som finns var

Köpa: Många böcker finns väldigt billigt begagnade på [Abebooks](https://www.abebooks.com/)

## Skriva referenser

Många kurser saknar moment som involverar akademiskt skrivande, men när det väl gäller är det IEEE-stil som används:

* <https://libguides.murdoch.edu.au/IEEE/>
* <https://libguides.ust.hk/basic-citation/ieee-style>
* <https://guides.lib.monash.edu/citing-referencing/ieee>

Sök efter `ieee citation style` för massor av fler guider och exempel.

[Zotero](https://www.zotero.org/) (som kan integreras med LibreOffice) kan vara nyttigt. Institutionen har i skrivande stund ODT-mallar som standard...

## Ställa frågor

Att köra fast när du programmerar är inget konstigt. Var inte rädd för att ställa frågor. Men tänk på *hur* du ställer frågor! Var inte rädd för att visa kod. Ge tillräckligt mycket information för att folk ska ha en sportslig chans att faktiskt kunna hjälpa dig, annars blir det lätt en tidsödande gissningslek. Se t.ex. [How to create a Minimal, Reproducible Example](https://stackoverflow.com/help/minimal-reproducible-example).

Har du ett GitHub-konto kan du klistra in kod i en [gist](https://gist.github.com/) och länka (gists kan tas bort senare). Annars kan du använda någon pastebin-sajt (<https://hastebin.com/>, <https://paste.ubuntu.com/> osv).

Mindre kodsnuttar kan du posta direkt på Discord. Se till att omge dem med  tre backticks - \`\`\`  - före och efter. T.ex.:

    ```
    kod kod kod
    kod kod kod
    ```

För syntax highlighting kan du även ange språk. T.ex.:

    ```cpp
    std::cout << "C++-kod weee" << std::endl;
    return 0;
    ```

Vilket då kommer visas som:

```cpp
std::cout << "C++-kod weee" << std::endl;
return 0;
```

## Mjukvara

### IDE:er och texteditorer
[JetBrains](https://www.jetbrains.com/) har en mängd populära IDE:er för olika språk (C++, Java, PHP, JavaScript, Python, etc). De funkar alla på såväl Linux och Windows som Mac. Kostar normalt $$, **MEN** är [gratis för studenter](https://www.jetbrains.com/student/) (använd din studentepostadress när du skapar konto).

[Sublime Text](https://www.sublimetext.com/) (Linux/Windows/Mac) är ett trevligt alternativ om din dator krackelerar under tyngden av JetBrains-programmen. Proprietärt, men obegränsad trial.

[vim](https://www.vim.org/) och [Emacs](https://www.gnu.org/software/emacs/) är fria, finns för alla plattformar under solen, har funnits i flera decennier och stora skaror fanatiska användare. [Spacemacs](http://spacemacs.org/) för de två religionerna samman en smula: Emacs med Vim-keybindings per default.

[Visual Studio Code](https://code.visualstudio.com/) (Linux/Windows/Mac) är ett snabbt och smidigt open-source alternativ som erbjuder många funktioner som traditionellt sett inte finns i texteditorer, som t.ex inbyggd terminal och stöd för versionskontroll.

#### Language Server Protocol
[Language Server Protocol](https://langserver.org) är ett protokoll där tanken är att olika editors ska kunna ta del av samma språkverktyg och stöds av ex Microsoft, IBM, Red Hat, Facebook mfl. Principen är ganska enkel, i editorn installerar du ett plugin som fungerar som klient, sedan installerar du en server för de programspråk du använder i ditt operativsystem. Klienten använder då aktuell server för att implementera de funktioner som stöds av servern. Det gör att ex även Vim, Emacs, Sublime Text etc på ett enkelt sätt kan använda funktionalitet ifrån projekt med stort stöd inom respektive community. Se länken ovan för klient-/serveralternativ för olika editors och språk.

**Förslag på klienter till vim**

Plug-and-play lösningar som inte kräver så mycket konfiguration
 * [ALE](https://github.com/dense-analysis/ale)
 * [coc-nvim](https://github.com/neoclide/coc.nvim)

För en lättviktsvariant som kräver lite konfigurering för varje språk
* [LanguageClient-neovim](https://github.com/autozimu/LanguageClient-neovim)

Samtliga klienter ovan är ganska väldokumenterade och har ett ganska stort antal användare.

### Linux

Vilken som helst av de stora, vanligt förekommande distributionerna ([Ubuntu](https://ubuntu.com/) / [Mint](https://www.linuxmint.com/) / [Debian](https://www.debian.org/), [Fedora](https://getfedora.org/), [Arch](https://www.archlinux.org/), osv. etc.) funkar bra för allt du kommer behöva göra under programmet. Senaste LTS-versionen av Ubuntu (LTS = long term support) är standardtipset: lätt att komma ihång med och populärast (så lätt att googla problem).

Att ha en dator med enbart Linux är rekommenderat (eller dual-boota om du orkar mecka). Annars kan du använda [VirtualBox](https://www.virtualbox.org/) (Linux/Mac/Windows), men det kommer att gå segare. Ett annat alternativ, om du kör Windows, är [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/about).

## Användbara länkar för olika programmeringsspråk

### Allmänt

* [Stack Overflow](https://stackoverflow.com/questions) är en frågor-och-svar-sajt som är en fullkomlig guldgruva för såväl studenter som yrkesverksamma för allt programmeringsrelaterat. Kört fast? Prova googla `site:stackoverflow.com hur gör jag X`. Se även [de andra sajterna i Stack Exchange-nätverket](https://stackexchange.com/sites#) såsom [Server Fault](https://serverfault.com/) (för system- och nätverksadmins), [Super User](https://superuser.com/) ("for computer enthusiasts and power users"), [Ask Ubuntu](https://askubuntu.com/) osv.
* [Compiler Explorer (godbolt.org)](https://godbolt.org/) - "interactive online compiler which shows the assembly output of compiled C++, Rust, Go (and many more) code" - smidigt för att jämföra vad olika språk och kompilatorer (eller olika optimeringsnivåer i samma kompilator) faktiskt genererar i slutändan för en viss kodsnutt. Se även Matt Godbolts föredrag [“What Has My Compiler Done for Me Lately? Unbolting the Compiler's Lid”](https://www.youtube.com/watch?v=bSkpMdDe4g4) från CppCon 2017.

### C++

* [Cppreference](https://en.cppreference.com/w/cpp) - Väldigt användbar referens för C++ och standard biblioteket. Ibland lämnar sökfunktionen en del att önska. Om du inte hittar det du söker så använd en vanlig sökmotor, då de första träffarna på sökningar innehållandes "C++" brukar komma härifrån. Något bättre uppdaterad än [Cplusplus.com](http://www.cplusplus.com/).
* [Cpp Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) - En samling generella riktlinjer där målet är modern kod som undviker vanliga fallgropar. Introducerad av Bjarne Stroustrup och Herb Sutter, två stora namn inom C++ communityt. Behandlar väldigt mycket och allt är inte relevant för nybörjarkurser men kan vara väl värt att snegla på då och då för den som är intresserad. Om begrepp som klasser och funktioner är nya för dig så finns det annat att fokusera på.

### JavaScript, CSS, HTML

Olika saker men tenderar att användas tillsammans i kurserna på programmet.

* Mozillas [MDN](https://developer.mozilla.org/) är en pålitlig källa för tutorials och referensmaterial och annat för [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML), [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS), [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), etc.
* [caniuse.com](https://caniuse.com/) är bra för att se exakt vad olika webbläsare stöder.

## Kurser år 1

### DT013G Datavetenskaplig introduktionskurs

### DT158G Operativsystem introduktion, med tillämpningar i Linux

* [linuxjourney](https://linuxjourney.com/) - Kom igång med Linux - guider på olika nivåer
* [Extramaterial: Operating System Concepts](https://www.os-book.com/) - Slides, sammanfattningar, anteckningar m.m. för alla kapitel i kursboken av Silberschatz
* [Stallings ppt slides](https://s2.smu.edu/~devans/7343/OS9epptSlides/) - Slides för kursboken av Stallings, med detaljerad förklaring till varje bild
* [Umask-värden](https://www.linuxtrainingacademy.com/all-umasks/) - En sammanställning av alla kombinationer för umask med resulterande behörigheter

### DT018G Introduktion till programmering i C++

* [The Definitive C++ Book Guide and List](https://stackoverflow.com/questions/388242/the-definitive-c-book-guide-and-list)

### DT151G Datorkommunikation och nätverk, med tillämpningar i Linux

### DT019G Objektbaserad programmering i C++

Du kan använda vad som helst, men en IDE såsom CLion eller Visual Studio kan vara väldigt hjälpsam.

### MA140G Diskret matematik för programmerare

* [Matteboken.se](https://www.matteboken.se/) - gratis övningar och lektioner. Speciellt Matte 5 och Mattespecialisering tar upp saker relevanta för kursen.
* [Symbolab Math Solver](https://www.symbolab.com/) - förklarar hur godtycklig ekvation kan lösas

### DT076G Databaser, modellering och implementering

* [DB Browser for SQLite](https://sqlitebrowser.org/) (sqlitebrowser) - "visual, open source tool to create, design, and edit database files compatible with SQLite" - snabbt och enkelt sätt att laborera med databaser

### DT060G Objektorienterad programmering i C++

## Kurser år 2

### DT042G Metoder och verktyg i mjukvaruprojekt

* [Oh, shit, git!](https://ohshitgit.com/) - lösningar på vanliga problem

### DT074G XML

### DT062G Java för C++ programmerare

Använd IntelliJ IDEA (gratis studentlicens) för att göra livet drägligare.

### DT146G Webbprogrammering med HTML5, CSS3 och JavaScript

Lär dig använda developer tools i Firefox eller Chrome. Ovärderligt/oumbärligt.

### DT063G Designmönster med C++

### DT161G Webbprogrammering med PHP och PostgreSQL

* [PHP: The Right Way](https://phptherightway.com/) ("There’s a lot of outdated information on the Web that leads new PHP users astray, propagating bad practices and insecure code. PHP: The Right Way is an easy-to-read, quick reference for PHP popular coding standards, links to authoritative tutorials around the Web and what the contributors consider to be best practices at the present time.")

### DT031G Applikationsutveckling för Android

### DT167G Mjukvarusäkerhet

## Kurser år 3

### DT166G Presentation av ny teknik

### DT065G Systemprogrammering i UNIX/Linux

### DT045A Java Enterprise-utveckling med EE-standarden

Numera ersatt av DT176G Reaktiv programmering / RxJava?

### DT147G Programmering med samtidighet och parallellism

### DT015A Artificiell Intelligens för agenter

### DT002G Tillämpad datateknik, mjukvaruprojekt

### DT133G Sjävständigt arbete

## Annat nyttigt

### Studentombud och rättigheter

Studentkåren i Östersund har ett heltidsanställt [studentombud](http://www.studentostersund.se/utbildning/studentombudet/) som kan hjälpa dig vid problem med universitetet. ("Alla studenter på Mittuniversitetet i Östersund kan få råd och medlemmar i kåren får dessutom ytterligare hjälp i form av att studentombudet företräder dem i ärendet om så önskas. Kårmedlemskapet ger det lilla extra.")

Mittuniversitetets [regel för examination](https://medarbetarportalen.miun.se/globalassets/styrdokument/3.-utbildning-pa-grund-och-avancerad-niva/utbilda/bilaga-till-miun-2016-1998-regel-for-examination.pdf) säger bland annat:

> Rättningstiden för examination vid Mittuniversitetet är högst 15 arbetsdagar. Rättningstid räknas från dagen efter examinationstillfället tills den dag resultatet redovisas. Om särskilda skäl föreligger kan avdelning besluta om undantag från denna regel efter samråd med berörda studenter.

och:

> Datum för ny examination ska meddelas senast vid ordinarie examinationstillfälle. Tiden mellan meddelandet av resultatet av examinationen och ny examination måste vara minst två (2) kalenderveckor.

Se även Universitetskanslerämbetets vägledning [Rättssäker examination](https://www.uka.se/publikationer--beslut/publikationer--beslut/vagledningar/vagledningar/2017-07-06-rattssaker-examination.html).

### Studenterbjudanden/-rabatter

* [JetBrains](https://www.jetbrains.com/student/)-programmen (se IDE:er ovan) - få samtliga gratis
* [GitHub Student Developer Pack](https://education.github.com/pack) - allt möjligt, t.ex. $X i kredit på diverse molntjänster, samt Pro-konto på GitHub (ingen större skillnad jämfört med gratiskontot, men det står då "PRO" i din GitHub-profil! Whoa!). Bör räcka med att du använder din @student.miun.se-adress för verifiering, inget mer än så krävs.
* [Dustin Home](https://www.dustinhome.se/student) har studentrabatter
* [Lenovo](https://www.lenovo.com/se/sv/studentrabatt/) har studentrabatter (Thinkpad X- eller T-serie standardtips för bra utvecklarlaptops)
* [Dell](https://www.dell.com/sv-se/shop/dell-advantage/cp/students) har studentrabatter (XPS-serien är mycket populär bland utvecklare, kan ibland fås förinstallerad med Linux)
* [Apple](https://mecenat.com/se/apple) har studentrabatter (MacBooks är också väldigt populära bland utvecklare)
* [Microsoft Office 365](https://www.microsoft.com/en-us/education/products/office) Word, Excel och PowerPoint gratis för studenter
* [Tableau](https://www.tableau.com/academic/students) är ett program för analys och häftig visualisering av data. 1 års gratislicens för studenter genom din @student.miun.se-adress
* Se [Mecenat](https://mecenat.com/se) för allt möjligt annat

## Ändra den här sidan

Nåt som är fel? Nåt du vill lägga till? Den här sidan finns i ett [GitHub-repo](https://github.com/andersju/programvaruteknik). Gör en pull request! (Eller hojta på Discord.)

[Kramdown](https://kramdown.gettalong.org/syntax.html) används som syntax.
