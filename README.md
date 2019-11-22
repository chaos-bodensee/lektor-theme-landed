 lektor theme landed
=====================

For general Installation Instructions please have a look at [getlektor.com/docs/themes/installing](https://www.getlektor.com/docs/themes/installing/).

 Installation
--------------
1. Create ``themes`` Folder in your lektor project
2. The Folders ``templates``, ``models`` and ``flowblocks`` should be absent.
*Further investigation which folders may be present is needed!*
3. Add this template *(as git submodule)* into the ``themes`` folder.
4. copy and modify the ``example_settings.ini`` to ``databags/settings.ini``
5. copy and modify the ``example_scss.ini`` to ``configs/scss.ini``
6. The plugin ``lektor-scss`` should be present in your lektorproject
7. Maybe you want to add some alternative into your .lektorproject file

### shell instructions for installation
```bash
# first we need the themes folder
mkdir themes

# secound we delete some folders
# don't forget to have you have a copy of all files you need to keep!
rm -r templates models flowblocks assets

# add this template as gitmodule
git submodule add https://github.com/chaos-bodensee/lektor-theme-landed.git \
  templates/lektor-theme-landed

# copy the template settings
mkdir databags
cp templates/lektor-theme-landed/example_settings.ini \
  databags/settings.ini
# modify settings
nano databags/settings.ini

# copy the example_scss.ini
mkdir configs
cp templates/lektor-theme-landed/example_scss.ini \
  configs/scss.ini

# add plugin lektor-scss
lektor plugin add lektor-scss

# add english and saxon translation and german as default
cat templates/lektor-theme-landed/example_lektorproject.ini
nano *.lektorproject
```



 Inspiration
------------------
Design Inspired by [html5up.net/landed](https://html5up.net/landed)<br/>
Landed Design created by [AJ](http://twitter.com/ajlkn) under the [LICENSE](https://html5up.net/license) [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)


 Licence
-----------
```
Copyright (C) 2019 Max Bachmann
Copyright (C) 2019 L3D <l3d@c3woc.de>
Copyright (C) 2019 Toolbox Bodensee e.V. <kontakt@toolbox-bodensee.de>
Copyright (C) 2019 Chaos Bodensee

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

https://github.com/chaos-bodensee/lektor-theme-landed/blob/master/LICENCE
```
