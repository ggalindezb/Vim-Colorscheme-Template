# Colorscheme template

This is a template to create Vim colorschemes. It includes the most common
options used for a filetype independent colorscheme for a terminal Vim with 256
colors. Every option is set to default values, to create your colorscheme you
should fill in the necesary options.

## Highlight format

Every highlight group includes the following (obvious, already known) format:

    hi (Group)          ctermfg=none    ctermbg=none    cterm=none

Where:

- *Group.* The targeted highlight group. If you want to know what's exactly
  supposed to do, `:help highlight` or `:help hl-(Group)`
- *ctermfg.* The color of the letter of the syntax group.
- *ctermbg.* The color of the background of each letter in the syntax group.
- *cterm.* Formatting options. For a list of options, check `highlight-args` in
  `:help :highlight`

Every other colorscheme I came across came with most of the options, but without
a real order. It seems that someone did an original template with those options,
published it and then everybody else copied it. Being an order-paranoid, I
decided to tidy it up a bit.

## Order of the syntax groups

- **Editor settings.** Configuration regarding Vim's interface, not related to a
  given programming language.
    - *Number column.* The column with the line numbers and folds
    - *Window/Tab delmiters.* The area that shows window splits and opened tabs.
    - *File Navigation / Searching.* Just what the name says. 
    - *Prompt/Status.* What the name implies.
    - *Visual aid.* Matching parenthesis, visual block selection...
- **Variable types**
