# JayStack

**JayStack is a combination of two boilerplates; JayPack and JayCraft.**

Built by [@JayBox325](https://twitter.com/JayBox325) to help scaffold projects to speed up delivery of work including all the tools needed for a good quality build.

For the frontend structure, there's [JayPack](https://github.com/jaybox325/jaypack). It's a [Gulp 4](https://gulpjs.com/) framework with a [WebPack 4](https://webpack.js.org/) bolt-on to manage all the Javascript ES6 compilation.

With other features like [TailwindCSS](https://tailwindcss.com/) for utility-first CSS, effective asset optimisation and SVG symbols for scalable iconography.

Built to work hand-in-hand with [CraftCMS](https://craftcms.com/) (or more specifically: JayCraft), all the source files are compiled and output in a `/build` directory.

Once a new project is setup with JayPack, JayCraft can be cloned into the `/build` directory for a new CraftCMS instance with all the basics already set up.