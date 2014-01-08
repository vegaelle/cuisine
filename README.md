# cuisine.git

KISS Repository of open recipes. Simply find or write your personal recipes in
the recipes folder, in the MIAM (Miam Inside Advanced Markdown) syntax.
A Python script, cuisine.py, helps you finding the perfect recipe for your
meals. The options list is available by typing `./cuisine.py --help`.

## But… WHY??

Because I’m hungry. Everytime. “Cuisine” is the french for “kitchen/cooking”,
and “miam” is also the french for “yum” (this is not fedora-related, AFAIK).
Also, there are a lot of websites that show open source recipes, but those lack
a simple format for the raw data.

## MIAM syntax

A MIAM file is basically a text file following the
[Markdown](http://daringfireball.net/projects/markdown/) rules. In addition of
those, you can use metadata to help good indexing of the recipe.
The category of a recipe is given by its parent folder. Its language is given by
the extension (for example, tartiflette.en.miam for the recipe for *tartiflette*
in english).

## cuisine.py options

--random: selects and shows a random recipe that meet the optional criterias. If
  not specified, the full list of corresponding recipes will be shown

--with=<list,of,ingredients>: comma-separated list of ingredients that **must**
  be found in the recipe
  
--without=<list,of,ingredients>: comma-separated list of ingredients that **must
  not** be found in the recipe

--veggie, --vegan, --hallal […]: returns recipes that fit given culture only

--category=<cat>: returns recipes in the given category only

--keyword=<keyword>: returns recipes that contains the given keyword(s) (can be
  a list of comma-separated values)

--get=<name>: shows the recipe <name>
