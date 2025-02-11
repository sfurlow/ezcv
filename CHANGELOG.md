# Changelog

## V0.2.2; August 2nd 2021

Documentation bugs after release

### Bug fixes

- Fixed issue with mkdocs build not recognizing correct URL and image paths


## V0.2.1; August 2nd 2021

Fixed bugs after release

### Bug fixes
- Fixed the fact that colored was not included as setup.py dependency


## V0.2.0; August 2nd 2021

The focus for this release is to add new features and themes

### Features

- Added Resume Generator
- Setup remote theme support
- Added new section; gallery
  - Supports multiple images being put together into a gallery
- Google analytics config option
- Custom Favicon 
- Added new section creation CLI
- When initializing with a theme that is not downloaded it will try to be downloaded on initialization instead of first build
- Added support for all standard markdown file extensions (.md, .markdown, .mdown, .mkdn, .mkd, .mdwn)
- Added support for many image file extensions as content (.jpg, .png, .jpeg, .gif, .svg, .webp, .apng, .jfif, .pjpeg, .pjp)
- Added many new markdown extensions
  - [footnotes](https://python-markdown.github.io/extensions/footnotes/)
  - [tables](https://python-markdown.github.io/extensions/tables/)
  - [toc (Table of contents)](https://python-markdown.github.io/extensions/toc/)
  - [abbr(abbreviations)](https://python-markdown.github.io/extensions/abbreviations/)
  - [def_list(Definition lists)](https://python-markdown.github.io/extensions/definition_lists/)
  - [sane_lists(Sane lists)](https://python-markdown.github.io/extensions/sane_lists/)
  - [mdx_math(Latex/formulas)](https://github.com/mitya57/python-markdown-math)
- Created filters module for creating custom Jinja filters (will be an exposed API for adding your own in v0.3.0)
- [Created several custom filters for optimizing & simplifying theme development](https://ezcv.readthedocs.io/en/latest/theme-development/#available-custom-filters)
    - [split_to_sublists; Takes a list and splits it into sublists of size n](https://ezcv.readthedocs.io/en/latest/theme-development/#split_to_sublists)
    - [get_image_path; Takes in the path to an image and returns it in usable format to use in img tags as src attribute](https://ezcv.readthedocs.io/en/latest/theme-development/#get_image_path)
    - [get_filename_without_extension; Takes in path and returns filename without extension](https://ezcv.readthedocs.io/en/latest/theme-development/#get_filename_without_extension)
    - [pretty_datetime; A utility function for pretty printing dates provided for jobs/getting a degree/volunteering etc](https://ezcv.readthedocs.io/en/latest/theme-development/#pretty_datetime)
    - [pretty_defaultdict; Returns a prettyprinted form of a defaultdict](https://ezcv.readthedocs.io/en/latest/theme-development/#pretty_defaultdict)

### Themes

- Moved existing themes to new repo https://github.com/QU-UP/ezcv-themes
- Added new themes
  - [cv](https://ezcv.readthedocs.io/en/latest/included-themes/#resume)
  - [Grayscale](https://ezcv.readthedocs.io/en/latest/included-themes/#grayscale)
  - [Paradigm Shift](https://ezcv.readthedocs.io/en/latest/included-themes/#paradigm-shift)
  - [Lens](https://ezcv.readthedocs.io/en/latest/included-themes/#lens)

### Bug fixes

- Fixed markdown files with different standard extensions not being recognized
- Fixed markdown files with capitalized extensions not being recognized

### Documentation Improvements

- Added documentation for new features
- Added additional onboarding videos/tutorials
- Added section for finding help/support

## V0.1.1; January 10th 2020

Fixes following initial launch

### Bug fixes

- Added additional warnings for if necessary config value is not provided

### Documentation improvements

- Updated necessary docstrings

## V0.1.0; January 10th 2020

Initial release of ezcv

### Features

- Themes Added:
  - [aerial](https://html5up.net/aerial)
  - base
  - [creative](https://startbootstrap.com/theme/creative)
  - [dimension](https://html5up.net/dimension)
  - [ethereal](https://html5up.net/ethereal)
  - [freelancer](https://startbootstrap.com/theme/freelancer)
  - [Identity](https://html5up.net/identity)
  - [Read only](https://html5up.net/read-only)
  - [Solid State](https://html5up.net/solid-state)
  - [strata](https://html5up.net/strata)
- Added initial [example site](https://github.com/Descent098/ezcv/tree/master/ezcv/example_site)
- Added initial [CLI](https://ezcv.readthedocs.io/en/latest/cli/)
- Added initial [core files](https://github.com/Descent098/ezcv/blob/master/ezcv/core.py#L289-L402)
- Added to [pypi](https://pypi.org/project/ezcv/)

### Documentation improvements

- Added initial [api docs](https://kieranwood.ca/ezcv)
- Added initial [user docs](https://ezcv.readthedocs.io)
