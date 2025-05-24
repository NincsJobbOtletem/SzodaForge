# SzodaForge Minecraft Szerver v2

Ez a leírás tartalmazza a SzodaForge Minecraft szerver fájljait, konfigurációit és használt pluginok listáját a parancsaikkal.

---

## Használt Pluginok és Parancsaik

### Advanced-Portals-Spigot
- `/ap create <név>` - Új portál létrehozása aktuális pozíción.
- `/ap link <név> <világnév/koordináták>` - Portál összekapcsolása világ vagy koordinátákkal.
- `/ap delete <név>` - Portál törlése.
- `/ap setteleport <név>` - Teleport célpont beállítása az aktuális pozícióra.
- `/ap reload` - Konfiguráció újratöltése.

### AuraSkills
- `/skills` - Képességek menü megnyitása.
- `/skills stats [játékos]` - Képesség statisztikák megtekintése.
- `/skills levelup <képesség> <szint>` - Képesség szintlépése (admin).
- `/skills reset [játékos]` - Képességek visszaállítása (admin).
- `/skills info <képesség>` - Képesség információk.

### CMILib
- `/cmi check [játékos]` - Játékos információk (IP, online idő).
- `/cmi heal [játékos]` - Gyógyítás.
- `/cmi feed [játékos]` - Jóllakatás.
- `/cmi repair [all]` - Eszközök javítása.
- `/cmi kit <név> [játékos]` - Kit átadása.
- `/cmi scan` - Eltűnt blokkok felkutatása.
- `/cmi tps` - Szerver TPS mutatása.

### DecentHolograms
- `/dh create <név> <szöveg>` - Hologram létrehozása.
- `/dh addline <név> <szöveg>` - Sor hozzáadása hologramhoz.
- `/dh removeline <név> <sor_szám>` - Sor eltávolítása.
- `/dh movehere <név>` - Hologram mozgatása aktuális pozícióra.
- `/dh delete <név>` - Hologram törlése.
- `/dh list` - Hologram lista.

### Dynmap
- `/dynmap hide` - Játékos elrejtése a térképről.
- `/dynmap show` - Játékos megjelenítése.
- `/dynmap render` - Térkép újrarenderelése.
- `/dynmap fullrender` - Teljes térkép renderelése.
- `/dynmap reload` - Konfiguráció újratöltése.

### EconomyShopGUI
- `/shop` - Bolt menü megnyitása.
- `/shop reload` - Bolt konfiguráció újratöltése.
- `/shop open <bolt_id> [játékos]` - Specifikus bolt megnyitása.
- `/shop editor` - Bolt szerkesztő (admin).
- `/shop save` - Bolt konfiguráció mentése.

*(és így tovább, a többi plugin is hasonló módon)*

---

## Docker Compose alap parancsok

A szerver futtatásához Docker Compose-t használunk.

- **Szerver elindítása:**
  ```bash
  docker-compose up

