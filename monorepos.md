
---

## Monorepos

Instead of relying on binaries, monorepos depends directly on the source code of the modules it depends on.

One advantage of a monorepo is the sharing of common 3rd party libraries. For instance, module A and module B both rely on  third party library X. Then, they only have to install the library once. All libraries in a monorepo is installed on the root folder.

But don'tmake the mistake that if a company adopts a monorepo approach, it will have only one repo for the whole company.

Monorepos are meant for related modules, which share common versioning. A good example is Babel, which have loads of components, mostly plugins. It has a Babel-core, Babel-preset-env, Babel-react-plugin, etc. Before Babel switched to a monorepo,  these 3 components have different version numbers. Now that they use the same versioning, users of these plugins would now know if they are using the latest version of Babel or not.

There are two types of monorepos. The Monstrous Monorepos and the project monorepos. The Monstrous Monorepos is the single repository of a company, which includes both related and unrelated components. Project monorepos only contain related components.

**Making large scale refactorings**

This is easier in a monorepo, but pretty difficult to implement in a non-monolithic environment. Say we are changing the api of a core library, therefore, we also need to change other libraries that depend on it. In a monolithic environment, there will be just one commit for all modules.

**Single CI**

Imagine if you have multiple websites that share a common library. In a non monolithic environment, you will need to deploy each of these websites separately. Now, with a monorepo, you deploy once, and all your websites will get deployed automatically. Because there is only one repository. The disadvantage of this is that if you make a change on just one website and deploy, all your websites will get deployed again even though there is really no change in them. But I think this could be solved by modifying some config on your CI environment. Like implementing a conditional NO-OP if that particular site didn't change at all.

