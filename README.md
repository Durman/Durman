Hello, I'm one of the [Sverchok](https://github.com/nortikin/sverchok) developers since 2017. Sverchok is open source add-on for procedural modeling in Blender. First of all it's great tool to learn how procedural workflow works. At the moment of writing it has more than 700 nodes which reveal a lot of possibilities. I'm learning procedural workflow myself and trying to improve Sverchok so new possibilities would be available to play for every one. My examples of usage sverchok you can find: [Twiter](https://twitter.com/SoluSerg), [ScketchFab](https://sketchfab.com/randum), [YouTube](https://www.youtube.com/channel/UCG0X2w4SETBI745pGK_Zccg).

Short history of my contribution to Sverchok:
- *2017 - 2020* In this period I mainly learned programming, algorithms, data structures, Python, Blender API. My new knowledges I tried to convert in new nodes and improving existing ones. For example in the end of 2017 I implemented my first node, [Offset line](https://github.com/nortikin/sverchok/pull/1958). Now I'm even a bit surprised that I had been able to do this with such poor knowledge of programming.
- *2020* With experience of previous years of development I started to rewrite (refactoring) different places of Sverchok to prepeare it for new core featrues. In the end of the year I finished to rewrite [Group nodes](https://github.com/nortikin/sverchok/pull/3713), known as Monads in Sverhock.
- *2021* First of all it's implementing of [new execution system](https://github.com/nortikin/sverchok/pull/4164) which removed some limitations of old one and with a lot of possibilities for future improvements. Secondly I started to be concerned about how Sverchok appear to the users what forced me made [documentation refactoring](https://github.com/nortikin/sverchok/pull/4220) and some other improvements.

Though a lot of work is done there are still a lot of thing to be improved:
- First of all I'm continuing to work on execution system. There are cool thing which would be nice and possible to have. For example [updating nodes upon changes in a scene](https://github.com/nortikin/sverchok/issues/4283), [freezing nodes](https://github.com/nortikin/sverchok/issues/4322), muting nodes, progress bar, improve cancelling work etc.
- Nodes inconsistency. One of the Sverchok problems is decentralized process of nodes developing. Each Sverchok developer has his own understanding of how nodes should work. So some similar nodes expect different data structure as input and have different data structure as output, has one vectorization rules some another some does not have them at all. 
- Nodes regression. Nodes improvements quite frequently can lead to breaking their work within old layouts.
- Performance
- UI problems

<!--
**Durman/Durman** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
