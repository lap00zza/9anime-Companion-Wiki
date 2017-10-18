1. Install NodeJS
2. Install git
3. Run the following commands
   ```bash
   # Clone the repository and move inside it
   $ git clone https://github.com/lap00zza/9anime-Companion.git
   $ cd 9anime-Companion

   # install dependencies
   $ npm install

   # Build the extension. If gulp command is not working, it means 
   # you dont have gulp-cli. You can either download gulp-cli or use
   # npm run build.
   $ gulp
   ```
4. Check `dist/chromium` and `dist/firefox` for the built extension.
5. *Optional:* since the project is in Typescript, be sure to use a editor like [VSCode](https://code.visualstudio.com/) to take full advantage.
6. *Optional:* check out the instructions for [Running in Developement Mode](https://github.com/lap00zza/9anime-Companion/wiki/Running-in-Developement-Mode)

> :information_source: Check `gulpfile.js` and `package.json` for all the available tasks