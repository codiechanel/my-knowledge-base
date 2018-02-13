## Monorepos

Instead of relying on binaries, monorepos directly to the source code of the modules it depends on.

One advantage of a monorepo is the sharing of common 3rd party libraries. For instance, module A and module B both rely on  third party library X. Then, they only have to install the library once. All libraries in a monorepo is installed on the root folder.

But don'tmake the mistake that if a company adopts a monorepo approach, it will have only one repo for the whole company.

Monorepos are meant for related modules, which share common versioning. A good example is Babel, which have loads of components, mostly plugins. It has a Babel-core, Babel-preset-env, Babel-react-plugin. Before Babel switched to a monorepo,  these 3 components have different version numbers. 

So if a module is not related at all, it should not be added to the monorepos. So in practice, 

