# TemplateParent
ProcessWire module that allows limiting templates for new pages based on the parent page

## Status

Beta - Proof-of-Concept, use at your own risk (though this shouldn't be too high as the module saves all settings in its own database table)

## Compatibility

Tested with ProcessWire 2.7 and 3.x, though it should also work on older versions. If it works for you on 2.5 or 2.6, please let me know.

## Usage

- Download ZIP file and extract it under site/modules in your ProcessWire installation
- In PW's backend, click on Modules -> Refresh
- Install TemplateParent (ProcessTemplateParent will be installed alongside)
- You'll find a new menu entry "Template Parents" under "Setup"
- On this page, assign possible parent pages to your templates
 
Restrictions entered here will be applied after the regular regular restrictions in the template's family settings are applied, which means you can't make an already excluded template visible in the drop-down list for new page through this method, only disallow otherwise allowed templates.

From version 0.0.6 on you can also edit allowed parents directly on the family tab of the template.

## Advanced

This module also supports inheritance, i.e. allowing a template for child pages if the template has been allowed for one of the parent's ancestors.

To enable this functionality, go to Modules -> Configure -> ProcessTemplateParents, check the box for inheritance and save.

Note that a permission once granted for a parent can't be revoked further down.

## License

Released under Mozilla Public License v2. See file LICENSE for details.
