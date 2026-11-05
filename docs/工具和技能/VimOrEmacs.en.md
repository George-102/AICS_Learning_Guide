# Vim and Emacs

## Why Learn Vim or Emacs

Vim and Emacs bring the following benefits:

- They keep your fingers on the keyboard for almost the whole development process: Vim's modal editing and Emacs's key binding system both revolve around the keyboard for cursor movement, text manipulation, and command execution, avoiding frequent switching between arrow keys and the mouse so your hands stay in an efficient input state.
- Convenient file switching and window/buffer management let you work on several files at once, or even several places in the same file: Vim has buffers, windows, and tabs, while Emacs has buffers, windows, and frames, and both organize multi-task editing comfortably.
- Vim's macros and Emacs's keyboard macros and Elisp scripts can batch repetitive work, such as indenting multiple lines, adding double quotes in bulk, or renaming in bulk, handing mechanical labor to the editor.
- Vim is the command line editor bundled with many servers, so after you connect to a remote server over `ssh` there is usually no graphical interface and Vim is ready to use; Emacs also runs in a terminal and can edit remotely through mechanisms such as TRAMP, making it equally suited to environments without a GUI.
- An extraordinarily rich plugin/extension ecosystem gives you the fanciest terminal editor combinations in the world: Vim has a huge plugin catalog and Emacs has a vast Elisp package ecosystem, and both can be reshaped into a development environment that fits your personal workflow.
- Deep customization: Vim is configured through `vimrc`, Vimscript, and Lua, while Emacs is configured through `init.el` and Elisp, and both can be polished into a personal tool.

## How to Learn

Unfortunately the learning curve for Vim (or Emacs) really is steep, and it took me several weeks to gradually get used to developing with Vim. At first it feels very uncomfortable, but once you get past the initial stage, believe me, you will love them.

Vim and Emacs are two editors older than most readers. Vim's predecessor vi was born in Berkeley in 1976, and Emacs's prototype appeared even earlier at MIT's AI Lab, where Richard Stallman later organized it into GNU Emacs. They survive today not out of nostalgia but because they held on long enough to a direction almost every editor has abandoned: break editing down into the smallest atomic operations composable from the keyboard, then let users assemble them.

Vim's answer is to split editing into "modes". In normal mode keys are not for typing characters but for actions: `d` is the delete operator, `w` is the text object "next word", so `dw` deletes one word, and `ci"` means "change the contents inside quotes". The benefit of this compositional grammar is unlimited derivation; once familiar, editing turns from character-by-character movement into a single operation on a structure. The price is a steep learning curve, with efficiency dropping noticeably in the first two weeks.

Emacs's answer is not modes but a programmable runtime environment. It is essentially a Lisp interpreter whose first application happens to be an editor, so key binding enumeration, buffers, windows, and even mail, calendars, and terminals all live under the same set of abstractions. This "editor as operating system" route gives Emacs almost no ceiling on customization, and org-mode grew out of that culture: a plain text markup format that nonetheless handles notes, to-dos, schedules, table calculations, and code block execution.

Neither is the easy choice. The point of this chapter is not to convince you to switch editors but to provide an ordered learning path so you can learn while using it in a real project instead of getting stuck in configuration. The most important principle when learning is: **learn to use it first, then learn to configure it**. Most Vim plugins merely wrap built-in features, and most Emacs distributions (such as Doom, Spacemacs, and Centaur) package other people's configurations for you, and applying them directly leaves you helpless when something breaks.

## Course Resources

- Vim course (Chinese): <https://wsdjeg.net/vim-galore-zh-cn/>
- Vim course (English): <https://learnvimscriptthehardway.stevelosh.com/>
- Emacs course (Chinese): the Zhihu column <https://www.zhihu.com/column/c_1440829147212279808>
- Vim practice: the interactive tutorial `vimtutor` bundled with Vim (a Chinese translation loads in a Chinese environment) is the first thing you should complete; it turns mode switching, deletion, pasting, movement, search, replacement, and file operations into a dozen hands-on lessons, and you should get through it smoothly before reading further.
- Emacs practice: the interactive `C-h t` tutorial (`help-with-tutorial`) bundled with Emacs covers cursor movement, the clipboard, windows, search, and file operations, and explains what the `C-h` prefix means. It is Emacs's counterpart to `vimtutor`.