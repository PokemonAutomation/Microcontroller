# Clothing Buyer

## Program Description

As its name implies, this program will automatically buy clothing.

### Setup of Settings

1. Text Speed: Fast
2. Casual mode: Off

### Instructions

1. You are in the menu for buying clothing. (Anywhere is fine.)
2. Start the program in the [Change Grip/Order Menu](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Appendix:-ChangeGripOrderMenu).

### Default Program Settings

This program is not particularly efficient, but will properly handle items that have already been purchased. It will eventually clear an entire store regardless of how many items there are in each category.

Preliminary testing suggests that this program takes an hour to buy out the entire Wedgehurst clothing store.

*Be aware that this program will change your clothing. So you may need to fix it when you’re done.*

   > Note that this program does not stop since it does not know when it is done. Therefore you must stop it manually and check to see if it there is anything left to buy.

***

### Options

This program uses [`TOLERATE_SYSTEM_UPDATE_MENU_FAST`](https://github.com/PokemonAutomation/SwSh-Arduino/wiki/Appendix:-GlobalSettings#tolerate-system-update-menu-fast) to bypass the system update window.

### Rotate Categories:
```
const bool CATEGORY_ROTATION    =   true;
```
When set to true, the program will change categories. This allows the program to eventually buy out the entire store, but will make it less efficient when there are categories that are already bought out.
