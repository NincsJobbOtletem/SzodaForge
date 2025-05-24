Aha, teljesen értem! A korábbi válasz is már Markdown formátumban volt (amit egy .md fájlba másolhatsz), de most összefoglalom az egészet egy blokkban, pontosan úgy, ahogy egy README.md fájlba illik.

Ezt az alábbi szöveget másold be egy README.md nevű fájlba a projekt gyökérmappájába:

Markdown

# SzodaForge Minecraft Szerver v2

Ez a leírás tartalmazza a SzodaForge Minecraft szerver fájljait, konfigurációit és a használt pluginok listáját a legfontosabb parancsaikkal.

---

## Használt Pluginok és Parancsaik

### Advanced-Portals-Spigot
* `/ap create <név>` - Új portál létrehozása az aktuális pozíción.
* `/ap link <név> <világnév/koordináták>` - Portál összekapcsolása egy másik világgal vagy konkrét koordinátákkal.
* `/ap delete <név>` - Portál törlése.
* `/ap setteleport <név>` - Teleport célpont beállítása az aktuális pozícióra.
* `/ap list` - Meglévő portálok listázása.
* `/ap info <név>` - Részletes információk egy portálról.
* `/ap reload` - Konfiguráció újratöltése.

### AuraSkills
* `/skills` - Képességek menü megnyitása.
* `/skills stats [játékos]` - Képesség statisztikák megtekintése egy játékosról (vagy magadról).
* `/skills levelup <képesség> <szint>` - Egy adott képesség szintlépése (admin parancs).
* `/skills reset [játékos]` - Képességek visszaállítása egy játékosnál (admin parancs).
* `/skills info <képesség>` - Részletes információk egy képességről.
* `/skills profession <játékos> <professzió>` - Játékos professziójának beállítása (admin parancs).
* `/skills debug` - Debug mód be- és kikapcsolása.

### CMILib (Ez egy segédplugin, számos hasznos funkcióval, elsősorban admin/mod parancsokat tartalmaz)
* `/cmi check [játékos]` - Játékos információk lekérdezése (IP, online idő, utolsó login, stb.).
* `/cmi heal [játékos]` - Játékos gyógyítása.
* `/cmi feed [játékos]` - Játékos jóllakatása.
* `/cmi repair [all/hand]` - Eszközök javítása (kézben lévő vagy az összes inventoryban lévő).
* `/cmi kit <név> [játékos]` - Kit átadása játékosnak.
* `/cmi warp <név> [játékos]` - Teleportálás egy előre beállított warp ponthoz.
* `/cmi setwarp <név>` - Warp pont létrehozása az aktuális pozíción.
* `/cmi delwarp <név>` - Warp pont törlése.
* `/cmi home [név]` - Teleportálás a saját otthonodba.
* `/cmi sethome [név]` - Otthon beállítása az aktuális pozíción.
* `/cmi delhome [név]` - Otthon törlése.
* `/cmi tps` - Szerver TPS (Ticks Per Second) mutatása.
* `/cmi broadcast <üzenet>` - Üzenet küldése a szerverre, mindenki látja.
* `/cmi vanish` - Láthatatlanná válás (admin/mod).
* `/cmi fly [játékos]` - Repülés be/ki kapcsolása (játékosnak is).
* `/cmi gamemode <mode> [játékos]` - Játékos játékmódjának váltása (pl. survival, creative).
* `/cmi scan` - Eltűnt blokkok felkutatása (admin/debug).
* `/cmi reload` - Plugin konfigurációjának újratöltése.

### DecentHolograms
* `/dh create <név> <szöveg>` - Hologram létrehozása egy kezdő szöveggel.
* `/dh addline <név> <szöveg>` - Sor hozzáadása egy hologramhoz.
* `/dh setline <név> <sor_szám> <új_szöveg>` - Egy meglévő sor tartalmának módosítása.
* `/dh removeline <név> <sor_szám>` - Sor eltávolítása a hologramból.
* `/dh movehere <név>` - Hologram mozgatása az aktuális pozícióra.
* `/dh teleport <név>` - Teleportálás a hologram pozíciójához.
* `/dh delete <név>` - Hologram törlése.
* `/dh list` - Összes hologram listázása.
* `/dh reload` - Konfiguráció újratöltése.

### Dynmap
* `/dynmap hide` - Játékos elrejtése a térképről.
* `/dynmap show` - Játékos megjelenítése a térképen.
* `/dynmap render` - Térkép újrarenderelése (a friss változások megjelenítéséhez).
* `/dynmap fullrender` - Teljes térkép renderelése (nagy erőforrásigényű, hosszú folyamat).
* `/dynmap cancelrender` - Folyamatban lévő renderelés megszakítása.
* `/dynmap pause` - Térkép frissítésének szüneteltetése.
* `/dynmap reload` - Konfiguráció újratöltése.

### EconomyShopGUI
* `/shop` - Bolt menü megnyitása.
* `/shop reload` - Bolt konfiguráció újratöltése.
* `/shop open <bolt_id> [játékos]` - Specifikus bolt megnyitása játékosnak.
* `/shop editor` - Bolt szerkesztő módba lépés (admin).
* `/shop save` - Bolt konfiguráció mentése.
* `/shop additem <ár_eladás> <ár_vétel>` - Tárgy hozzáadása a bolthoz a kézben lévő tárgy alapján (editor módban használható).

### EssentialsX (Ha ezt a plugint használjátok a CMILib helyett, vagy mellette a kiegészítő funkciókért)
* `/spawn` - Teleportálás a szerver spawn pontjához.
* `/setspawn` - Spawn pont beállítása (admin).
* `/tpa <játékos>` - Teleportálási kérés küldése egy játékosnak.
* `/tpaccept / tpdeny` - Teleportálási kérés elfogadása / elutasítása.
* `/home` - Teleportálás otthonhoz.
* `/sethome [név]` - Otthon beállítása.
* `/delhome [név]` - Otthon törlése.
* `/warp <név>` - Teleportálás warp ponthoz.
* `/setwarp <név>` - Warp pont létrehozása (admin).
* `/delwarp <név>` - Warp pont törlése (admin).
* `/bal / money` - Pénzösszeg megtekintése.
* `/pay <játékos> <összeg>` - Pénz küldése más játékosnak.
* `/baltop` - Leggazdagabb játékosok listája.
* `/msg <játékos> <üzenet>` - Privát üzenet küldése.
* `/r <üzenet>` - Válasz az utolsó privát üzenetre.
* `/god [játékos]` - Sebezhetetlenség be/ki kapcsolása.
* `/mute <játékos> [idő]` - Játékos némítása.
* `/kick <játékos> [ok]` - Játékos kirúgása.
* `/ban <játékos> [ok]` - Játékos kitiltása.
* `/jail <játékos> [idő] [ok]` - Játékos börtönbe zárása.
* `/unjail <játékos>` - Játékos kiszabadítása.
* `/give <játékos> <tárgy> [mennyiség]` - Tárgy adása játékosnak.
* `/item <tárgy> [mennyiség]` - Tárgy adása magadnak.
* `/clearinventory [játékos]` - Játékos inventoryjának kiürítése.
* `/time day/night` - Idő beállítása.
* `/weather clear/rain/thunder` - Időjárás beállítása.
* `/sundown / sunrise` - Napszak beállítása.
* `/setworth <tárgy> <érték>` - Tárgy értékének beállítása az economyban.

### GriefPrevention (Ha a telekvédelmi pluginot használjátok)
* `/claim` - Claim létrehozása az aktuális pozíción.
* `/trust <játékos>` - Játékos hozzáadása a claimhez, alapvető interakciós jogokkal.
* `/untrust <játékos>` - Játékos eltávolítása a claimből.
* `/accesstrust <játékos>` - Hozzáférési jog adása (pl. ajtók, gombok használata).
* `/containertrust <játékos>` - Konténer (ládák, kemencék) hozzáférési jog adása.
* `/permissiontrust <játékos>` - Játékosnak jog adása mások hozzáadására/eltávolítására a claimhez.
* `/subdivideclaims` - Alclaim mód bekapcsolása (nagyobb claimen belül kisebb, elkülönített területek).
* `/claimlist` - Claimjeid listázása.
* `/abandonclaim` - Aktuális claim elhagyása/törlése.
* `/abandonallclaims` - Összes claim törlése.
* `/buyclaimblocks` - Claim blokkok vásárlása.
* `/sellclaimblocks` - Claim blokkok eladása.
* `/claims` - Claim blokk statisztikák (hány blokkod van, mennyi a limit).
* `/trapped` - Segítség, ha elakadtál egy claimben, amiből nem tudsz kijutni.

### LuckPerms (Engedélykezelő rendszer)
* `/lp` - Fő parancs, nyitja a GUI-t (ha engedélyezve van és van hozzá jogosultság).
* `/lp user <felhasználónév> info` - Játékos engedélyeinek lekérdezése.
* `/lp user <felhasználónév> parent add <csoport>` - Játékos hozzáadása egy csoporthoz.
* `/lp user <felhasználónév> parent remove <csoport>` - Játékos eltávolítása egy csoportból.
* `/lp user <felhasználónév> permission set <permission> [true/false]` - Engedély beállítása/eltávolítása egy játékosnak.
* `/lp group <csoportnév> info` - Csoport engedélyeinek lekérdezése.
* `/lp group <csoportnév> permission set <permission> [true/false]` - Engedély beállítása/eltávolítása egy csoportnak.
* `/lp creategroup <név>` - Új csoport létrehozása.
* `/lp creategroup <név> parent set <szülő_csoport>` - Új csoport létrehozása szülő csoporttal.
* `/lp deletegroup <név>` - Csoport törlése.
* `/lp editor` - Engedélyek szerkesztése webes felületen keresztül (nagyon ajánlott adminoknak).
* `/lp applyedits` - Módosítások alkalmazása a webes szerkesztőből.
* `/lp reload` - Konfiguráció és engedélyek újratöltése.
* `/lp check <felhasználónév> <permission>` - Egy adott engedély ellenőrzése egy játékosnál.

### QuickShop-Hikari (Ha ezt a bolt plugint használjátok)
* `/qs` - Fő parancs, segítség.
* `/qs create` - Bolt létrehozása a kézben tartott tárggyal és összeggel (jobb gombbal kattintva egy ládára).
* `/qs sell` - Bolt beállítása csak eladásra.
* `/qs buy` - Bolt beállítása csak vételre.
* `/qs remove` - Bolt eltávolítása.
* `/qs setowner <játékos>` - Bolt tulajdonosának megváltoztatása (admin).
* `/qs toggle <bolt_ID>` - Bolt ki/bekapcsolása (admin).
* `/qs find <tárgy_név>` - Boltok keresése egy adott tárgyra.
* `/qs reload` - Konfiguráció újratöltése.
* `/qs clean` - Törölt boltok adatainak tisztítása.

### Vault (Ez egy API függőség, önmagában nincs sok parancsa, de fontos az economy és engedély rendszerekhez)
* `/vault` - Fő parancs, verzió információ.
* `/vault-eco` - Economy provider ellenőrzése.

---

## Docker Compose Alap Parancsok

A szerver futtatásához Docker Compose-t használunk, ami egyszerűsíti a szerver és a hozzá tartozó szolgáltatások kezelését.

* **Szerver elindítása:**
    ```bash
    docker-compose up
    ```
    *Ez a parancs elindítja a `docker-compose.yml` fájlban definiált összes szolgáltatást. Ha a háttérben szeretnéd futtatni, használd a `-d` (detach) opciót: `docker-compose up -d`.*

* **Szerver leállítása:**
    ```bash
    docker-compose down
    ```
    *Ez leállítja és eltávolítja a konténereket, hálózatokat és volume-okat, de a perzisztens adatok (ha volume-okkal vannak mountolva) megmaradnak.*

* **Szerver újraindítása:**
    ```bash
    docker-compose restart
    ```

* **Konzol hozzáférés:**
    A szerver konzoljához a következő paranccsal férhetsz hozzá (látod a naplókat és interakcióba léphetsz a szerverrel):
    ```bash
    docker-compose logs -f minecraft # A 'minecraft' a service neve a docker-compose.yml-ben
    ```
    Ha interaktív shellt szeretnél a konténeren belül (pl. fájlok szerkesztéséhez):
    ```bash
    docker-compose exec minecraft bash # A 'minecraft' a service neve a docker-compose.yml-ben
    ```

---

## A Projekt Felépítése / Fájlstruktúra

Ez a repository a következő fő mappákat és fájlokat tartalmazza:

.
├── docker-compose.yml       # A Docker Compose konfiguráció, ami definiálja a szerver konténerét és beállításait.
├── server/                  # A Minecraft szerver fő mappája.
│   ├── spigot.jar           # A szerver futtatható fájlja (pl. Paper.jar, Spigot.jar, stb.). Ezt a fájlt manuálisan kell ide helyezni.
│   ├── server.properties    # A Minecraft szerver alapvető beállításai.
│   ├── plugins/             # A szerver pluginjainak .jar fájljai és azok konfigurációs mappái.
│   │   ├── <plugin_neve>.jar
│   │   └── <plugin_neve>/    # Plugin konfigurációs mappák.
│   ├── world/               # Az alapvilág adatai (Overworld).
│   ├── world_nether/        # A Nether világ adatai.
│   ├── world_the_end/       # Az End világ adatai.
│   └── eula.txt             # A Minecraft EULA (End User License Agreement) elfogadását jelző fájl.
├── data/                    # Perzisztens adatok tárolására szolgáló mappa, ha Docker Volume-okhoz használod (pl. adatbázisok, extra konfigurációk).
├── .gitignore               # Fájlok és mappák listája, amelyeket a Git figyelmen kívül hagy.
└── README.md                # Ez a dokumentáció.


## Telepítés és Első Indítás

Kövesd az alábbi lépéseket a SzodaForge Minecraft szerver telepítéséhez és első indításához Docker Compose segítségével:

1.  **Docker és Docker Compose telepítése:**
    Győződj meg róla, hogy a Docker és a Docker Compose telepítve van a rendszereden. Utasításokat találsz a hivatalos Docker dokumentációban:
    * [Docker telepítés](https://docs.docker.com/get-docker/)
    * [Docker Compose telepítés](https://docs.docker.com/compose/install/)

2.  **Repository klónozása:**
    Nyiss egy terminált vagy parancssort, és klónozd ezt a repositoryt:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```
    *(Cseréld ki a `your-username` és `your-repo-name` részeket a tényleges GitHub felhasználónevedre és repository nevedre.)*

3.  **Minecraft szerver JAR fájl elhelyezése:**
    Töltsd le a kívánt Minecraft szerver JAR fájlt (pl. Paper, Spigot, Fabric, Forge) a hivatalos forrásból. Helyezd el ezt a fájlt a `server/` mappába. Győződj meg róla, hogy a `docker-compose.yml` fájlban a megfelelő fájlnév van beállítva a szerver indításához (általában `server.jar` vagy `spigot.jar`).

4.  **EULA elfogadása:**
    A Minecraft szerver indításához el kell fogadnod a Minecraft EULA-t. Hozz létre egy `eula.txt` fájlt a `server/` mappában, és írd bele a következő sort:
    ```
    eula=true
    ```

5.  **Szerver elindítása:**
    Navigálj a projekt gyökérkönyvtárába (ahol a `docker-compose.yml` található), és futtasd a szervert:
    ```bash
    docker-compose up -d
    ```
    *A `-d` (detach) opcióval a háttérben futtatod a szervert, így a terminál szabad marad.*

6.  **Konzol hozzáférés:**
    A szerver konzoljához a következő paranccsal férhetsz hozzá (látod a naplókat és interakcióba léphetsz a szerverrel):
    ```bash
    docker-compose logs -f minecraft # A 'minecraft' a service neve a docker-compose.yml-ben
    ```
    Ha interaktív shellt szeretnél a konténeren belül (pl. fájlok szerkesztéséhez):
    ```bash
    docker-compose exec minecraft bash # A 'minecraft' a service neve a docker-compose.yml-ben
    ```

## Karbantartás és Adminisztráció

* **Szerver leállítása:**
    ```bash
    docker-compose down
    ```
    *Ez leállítja és eltávolítja a konténert. A volume-ok (azaz a `server/` mappa tartalma) megmaradnak.*

* **Szerver újraindítása:**
    ```bash
    docker-compose restart
    ```

* **Pluginok frissítése / hozzáadása:**
    Helyezd el az új `.jar` fájlokat a `server/plugins/` mappába. A változások érvényesítéséhez indítsd újra a szervert (`docker-compose restart`).

* **Konfigurációs fájlok szerkesztése:**
    A szerver és a pluginok konfigurációs fájljai a `server/` mappán belül találhatók. Szerkesztés után (és ha szükséges) indítsd újra a szervert a változások érvényesítéséhez.

* **Biztonsági mentés:**
    A teljes szervermappa (`server/`) és az esetleges `data/` mappa rendszeres biztonsági mentése erősen ajánlott. Mivel a Docker volume-okat használunk, az adatok perzisztensek és könnyen menthetők egyszerű fájlmásolással.

## Portok

A következő portok vannak publikálva a `docker-compose.yml` fájlban:

* **25565/tcp:** Alapértelmezett Minecraft szerver port. Ezen keresztül csatlakoznak a játékosok.
* **8123/tcp:** Dynmap webes felület portja (ha engedélyezve van és ezen a porton fut). Ezen keresztül érhető el a szerver interaktív térképe böngészőből.
* *Adja hozzá ide az összes további portot, amit a `docker-compose.yml` fájlban publikál!*

---

## Hozzájárulás

Ha hibát találsz, vagy javaslatod van a szerverrel vagy a dokumentációval kapcsolatban:
* Nyiss egy "Issue"-t a GitHub repositoryban.
* Ha hozzá szeretnél járulni a kódhoz vagy a dokumentációhoz, nyiss egy "Pull Request"-et.

---

## Licenc

Ez a projekt a [Licenc típusa, pl. MIT] licenc alatt áll.
*(Cseréld ki a `[Licenc típusa, pl. MIT]` részt a tényleges licenc nevére, pl. MIT, GPLv3, st