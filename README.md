# Building your own Icebone

1. Install [cocopon/pgmnt.vim][pgmnt], a template engine for Vim color scheme,
   to your Vim.

2. To modify a color palette, edit `autoload/icebone/palette/(dark|light).vim`.
   If you make changes, be sure to `:source` this file before step 4 otherwise
   your color palette changes will not be reflected.

3. To modify highlighting groups or links, edit `src/icebone.vim`.

4. After editing, compile the source file as below:
 
5. 
   ### Ensure your file line endings are not converted to windows format. If so use following on each file:
   ```vim
       :w ++ff=unix 
   ```
   
   then:
   ```vim
   :e src/icebone.vim
   :cd %:h
   :source %
   ```

   Compiled files will be output into `autoload` directory.
