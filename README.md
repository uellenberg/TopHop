# TopHop
Link: https://www.desmos.com/calculator/lqr66vwfgf.

TopHot is a game for Desmos, written using [Graphgame](https://github.com/uellenberg/Graphgame) and [Logimat](https://github.com/uellenberg/Logimat). It's intended as a submission for Desmos' 2021 Math Art Competition, as well as a technical demo/example for Graphgame.

TopHop has an easy-to-use interface inspired by Geometry Dash.

## Graphgame and Logimat
Logimat is a language that compiles to Desmos (as well as pure math) which provides an interface intended to be as similar to a standard programming language as possible, and is based on Javascript. The core idea behind it is to simplify logical operations (for example, it includes standard if statements with comparison and boolean operators), but it also includes many features that help development, especially for someone who is not used to Desmos' syntax.

Graphgame is a game engine built on top of Logimat, and is based on Unity. It has concepts such as behaviors, game objects, and prefabs that allow for a data-driven approach to game development and makes code easily reusable. It also comes with several built-in behaviors that help to jump-start development.

## Graphgame Studio
[Graphgame Studio](https://graphgame.js.org) is a tool intended to make Graphgame development faster. It provides an integrated environment for editing code, compiling it, and putting it on Desmos. It also automates the process of styling elements, and comes with all the compilers and libraries you need built-in, so you don't need to set anything up to use Graphgame. Also, it includes basic git operations. If you'd like to explore this project and see how it works, I'd highly recommend using Graphgame Studio (also, make sure to read Graphgame and Logimat's documentation).

## Technology
TopHop is a showcase of Graphgame and Logimat's core systems, as well as some features that they ship with. As mentioned above, Graphgame and Logimat simplify the process of creating games and animations in Desmos, especially for those who are not used to how Desmos handles many things. They also allow for greater organization and cleaner code, by allowing for more granular control on how code is organized, separated, and commented, without providing a detrement for the compiled output.

Graphgame's behavior system also supplements this idea by allowing code to be split up into reusable packets (called behaviors), which can respond to input directly given to them (arguments), or variables on an object, and integrate with other components. For certain components that need to interact with others of the same kind (for example, colliders need to interact with other colliders), Graphgame provides systems that allow for dynamic code generation.

Graphgame and Logimat include quite a few features not listed here, and so I'd highly recommend taking a look at their documentation, as well as the code in this repository. Finally, these are some of the big components that Graphgame comes with:
- Rendering components that simplify the process of putting an object on the screen.
- Fast collision detection that's essential to any game or animation.
- DOA (Dynamic Object Allocation) system that allows several objects to be represented with only a few. For example, TopHop has 30 different world elements, but only needs 9 objects to represent them.

Logimat also allows code to be separated into different files.
