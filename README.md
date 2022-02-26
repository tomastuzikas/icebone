# Building your own Iceberg
NOTE: This section is for color scheme developers. If you just want to use the
color scheme, you don't have to follow these steps.

1. Install [cocopon/pgmnt.vim][pgmnt], a template engine for Vim color scheme,
   to your Vim.

2. To modify a color palette, edit `autoload/icebone/palette/(dark|light).vim`.
   If you make changes, be sure to `:source` this file before step 4 otherwise
   your color palette changes will not be reflected.

3. To modify highlighting groups or links, edit `src/icebone.vim`.

4. After editing, compile the source file as below:

   ```vim
   :e src/icebone.vim
   :cd %:h
   :source %
   ```

   Compiled files will be output into `autoload` directory.
