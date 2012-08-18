ReasonableRecipes
=================

ReasonableRecipes is a bukkit plugin that allows you to add crafting recipes. I originally created ReasonableRecipes to allow for more reasonable methods of repairing tools and armor, but this plugin's config is flexible enough to allow for defining many more recipes.

Configuration
-------------

When ReasonableRecipes loads for the first time, it will copy the default `config.yml` to `plugins/ReasonableRecipes/config.yml` if you do not already have a config. The default config contains recipes for repairing all tools and armors by combining the item with the tool's chief resource. For example, the defaults include a recipe to combine a damaged iron pickaxe with an iron ingot to craft a new unused iron pickaxe.

The ReasonableRecipes config currently supports one YAML node `shapeless-recipes` with a list of shapeless recipe formulas. For example:

    shapeless-recipes:
    - BOW = BOW + STRING
    - FISHING_ROD = FISHING_ROD + STRING

The shapeless recipe syntax reads like simple arithmetic assignment. The single item on the left of the equality is the recipe output, and the items on the right of the equality are the recipe inputs. Standard bukkit material names must be used in recipe definitions.

Version History
---------------

* *1.0*: Initial release with support for adding configurable shapeless recipes.
