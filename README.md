freight work
# ECO CARGO

FONTOS: Ha több karakteres rendszert használsz:

Kashakter esetén, ellenőrizd, hogy a client/main.lua fájlban az alábbi eseménykezelő tartlamazza a esx:kashloaded triggert
Az eco_cargo config fájlban állitsd a Config.kashacters = true értékre.

RegisterNetEvent('kashactersC:SpawnCharacter')
AddEventHandler('kashactersC:SpawnCharacter', function(spawn, isnew)

    -- Betöltési folyamat...
    -- ...
    -- ...

    TriggerEvent('esx:kashloaded')
end)


# MISSZIÓK

    Az alábbi listákat a config.lua-ban állitsd be

    -- rendfentartók listája:
        Config.lawEnforcementFactions

    -- Illegális frakciók listája:
        Config.illegalFactions



# PARANCSOK

    ADMIN:
    -- /cargodiag   -- Adatbázis karbantartás

    PLAYER:
    -- /inspect     -- A trailer mellé állva lekéri a szállítólevelet
    -- /mission     -- Küldetéslista
    -- /cargostat   -- Játékosok fuvar statisztikája
    -- /closenui    -- Nui bezárási problémák esetére

A szkriptbe építve megtalálható a mythic_notify így azt külön telepíteni nem kell.
