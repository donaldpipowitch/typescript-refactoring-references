This is an example to showcase a missing refactoring feature in TypeScript for projects which use multiple `tsconfig.json` files. I use VS Code to demonstrate the problem.

1. `$ git clone git@github.com:donaldpipowitch/typescript-refactoring-references.git`
2. `$ cd typescript-refactoring-references`
3. `$ yarn`
4. `$ cd packages/add`
5. `$ yarn build`
6. Open `packages/add/src/add.ts` in VS Code and `Rename Symbol` the exported function from `add` to `add2`.

`add` is not correctly renamed to `add2` inside `packages/use-add/src/use-add.ts`.