Title: Themes
Description: Each theme contains a set of content such as CSS files, layouts, etc. that apply to a specific recipe.
Order: 7
---
Each *theme* contains a set of content such as CSS files, layouts, etc. that apply to a specific recipe. A theme can be used to get up and running quickly with a given recipe by providing the set of resources the recipe requires. Because each recipe is a totally different set of modules, pipelines, metadata, etc. a given theme is only applicable to a specific recipe. The way a theme works is by providing an [input path](/docs/concepts/io#input-paths) that takes less precedence than the main input path. The theme itself is simply a bunch of files that would act the same way if they were sitting in your own `input` path.

# Overriding Theme Files

A byproduct of the layered input path design of themes is that it's easy to tweak how a theme works by simply overriding a file from the theme by placing an alternate version of the file with the same name and path inside your own `input` path. This version of the file will override the one from the theme. In fact, many themes take advantage of this behavior and contain blank files that exist only as extension points for individual sites to tweak the theme.   