## This is a feature branch for pokeemerald that adds a form of in-game printing for debugging purposes.

## Description of features:
To use this like a printf command, you only have to use an extern declare for DebugPrint.
You supply it an array of characters (string) to print, a number of arguments equal to the number of variables you want read out (can be zero if you just want to print text), and then every variable you want printed. 
You can load things into the StringVar buffers if you like, but this is intended to be used on the fly.
**DebugPrint((const u8[]) _("String to print"), NUM_VARS_TO_PRINT, var1, var2, var3) etc...**  

Open 'src/start_menu.c L#658 / L#609' to see an example of how to use it. You can see it ingame after compiling by opening then closing your start menu. It prints play time hours and minutes using DebugPrint when you close the start menu.

This branch eliminates much of the need for external debugging (using printf) such as mGBA printf, or similar. If you need multiline and logging, then you will want to use one of those solutions.

This can be fairly easily adapted to be usable in scripts just by supplying a script string as the 'buffer'.

Code for DebugPrint is in 'src/field_specials.c'
# ORIGINAL README.MD BELOW

# Pokémon Emerald

This is a decompilation of Pokémon Emerald.

It builds the following ROM:

* [**pokeemerald.gba**](https://datomatic.no-intro.org/index.php?page=show_record&s=23&n=1961) `sha1: f3ae088181bf583e55daf962a92bb46f4f1d07b7`

To set up the repository, see [INSTALL.md](INSTALL.md).


## See also

Other disassembly and/or decompilation projects:
* [**Pokémon Red and Blue**](https://github.com/pret/pokered)
* [**Pokémon Gold and Silver (Space World '97 demo)**](https://github.com/pret/pokegold-spaceworld)
* [**Pokémon Yellow**](https://github.com/pret/pokeyellow)
* [**Pokémon Trading Card Game**](https://github.com/pret/poketcg)
* [**Pokémon Pinball**](https://github.com/pret/pokepinball)
* [**Pokémon Stadium**](https://github.com/pret/pokestadium)
* [**Pokémon Gold and Silver**](https://github.com/pret/pokegold)
* [**Pokémon Crystal**](https://github.com/pret/pokecrystal)
* [**Pokémon Ruby and Sapphire**](https://github.com/pret/pokeruby)
* [**Pokémon Pinball: Ruby & Sapphire**](https://github.com/pret/pokepinballrs)
* [**Pokémon FireRed and LeafGreen**](https://github.com/pret/pokefirered)
* [**Pokémon Mystery Dungeon: Red Rescue Team**](https://github.com/pret/pmd-red)


## Contacts

You can find us on [Discord](https://discord.gg/d5dubZ3) and [IRC](https://web.libera.chat/?#pret).
