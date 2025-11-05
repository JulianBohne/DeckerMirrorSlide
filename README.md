# Mirror Explanation Slide

## Disclaimer
> This currently doesn't work properly in Firefox, as the MathJax inside the `<iframe>` is rendered wayyy to big.

## If you want to include this in another deck ...
1. ... copy the `julians-krams` and `support` directory to your project folder (should be in the root folder)
2. ... make sure to add the directories in the `static-resources`, as seen in the `decker.yaml`
3. ... copy the `mirror-content.md` file from the `mirror-slide` directory to a location of your choosing in your project
4. ... reference / include the `mirror-content.md` file, as seen in the `main-deck.md`
    > Note: Leave an empty line before / after the include so decker doesn't get confused
5. ... make sure to run this in Chrome (see disclaimer above)

## Useful Links
- [Documentation](https://decker.cs.tu-dortmund.de/decks/decker/manual/index.html)
    - Documentation as a Website or a PDF at the top
    - Documentation in Decker grouped by topics below

## Quickstart Guide
1. Download and install [Decker](https://decker.cs.tu-dortmund.de/)
    > More detailed instructions can be found [here](https://decker.cs.tu-dortmund.de/decks/decker/manual/index.html)
    1. Download the executable
        > Note: I'm using the current "latest" version (version: 0.14.0, branch: develop, commit: 698b000eed65930878e83ceccce6165ba84b4e94)
    2. Add it to your path environment variable
2. Run `decker --watch` in the `presentation` directory of this project
    > This will build the markdown files into the `public` folder and watch for changes to incrementally build the decks.
3. Run `decker serve` in the `presentation` directory of this project
    > This will start a web server (on port 8888)
4. Visit `localhost:8888` to view the compiled decks
5. Edit the markdown files in the `slide-sets` folder
    > This can be done in e.g. VSCode (there is also an extension pack `Decker Extension Pack`, that you might find useful)

## Project Structure
- `decker.yaml` (file)
    - This is the configuration file of this project. These settings can be overwritten in the header section of `...-deck.md` files.
    > Note: Math macros can be defined in here
- `main-deck.md` (file)
    - This is our presentation deck. It only includes all necessary parts from the other `.md` files.
- `support` (directory)
    - Contains third party dependencies (at the moment only `three.js`)
- `julians-krams` (directory)
    - Contains my `keyframe-plugin` that allows keyframing anything in an `iframe` using Reveil.js' fragments
    - Contains my `mathjax-morph` library used to transition one equation to another
    - Contains the main code for the mirror explanation slide

## Notes
- On some versions of decker, the `static-resources` property does not work. In these cases, try a different one (if that feature is important to you).
- There should be an empty line after an `[:import](...)` statement. Otherwise it doesn't work (at least not in the "latest" version)
