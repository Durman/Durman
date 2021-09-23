Hello, I'm one of the [Sverchok](https://github.com/nortikin/sverchok) developers since 2017. Sverchok is open source add-on for procedural modeling in Blender. First of all it's great tool to learn how procedural workflow works. At the moment of writing it has more than 700 nodes which reveal a lot of possibilities. I'm learning procedural workflow myself and trying to improve Sverchok so new possibilities would be available to play for every one. My examples of usage sverchok you can find: [Twiter](https://twitter.com/SoluSerg), [ScketchFab](https://sketchfab.com/randum), [YouTube](https://www.youtube.com/channel/UCG0X2w4SETBI745pGK_Zccg).

🕐 Short history of my contribution to Sverchok:
- **2017 - 2020** In this period I mainly learned programming, algorithms, data structures, Python, Blender API. My new knowledges I tried to convert in new nodes and improving existing ones. For example in the end of 2017 I implemented my first node, [Offset line](https://github.com/nortikin/sverchok/pull/1958). Now I'm even a bit surprised that I had been able to do this with such poor knowledge of programming.
- **2020** With experience of previous years of development I started to rewrite (refactoring) different places of Sverchok to prepeare it for new core featrues. In the end of the year I finished to rewrite [Group nodes](https://github.com/nortikin/sverchok/pull/3713), known as Monads in Sverhock.
- **2021** First of all it's implementing of [new execution system](https://github.com/nortikin/sverchok/pull/4164) which removed some limitations of old one and with a lot of possibilities for future improvements. Secondly I started to be concerned about how Sverchok appear to the users what forced me made [documentation refactoring](https://github.com/nortikin/sverchok/pull/4220) and some other improvements.

🎉 Though a lot of work is done there are still a lot of thing to be improved:
- **Excution system.** First of all I'm continuing to work on execution system. There are cool thing which would be nice and possible to have. For example [updating nodes upon changes in a scene](https://github.com/nortikin/sverchok/issues/4283), [freezing nodes](https://github.com/nortikin/sverchok/issues/4322), muting nodes, work with empty data, improve cancelling work etc. 
- **Nodes regression.** Nodes improvements quite frequently can lead to breaking their work within old layouts. To solve this problem [regression tests](https://github.com/nortikin/sverchok/pull/4253) can be implemented.
- **Performance**. Not everything but some aspects of Sverchok are slow. First milestone on this rode is [to fix one of the Sverchok architecture fault](https://github.com/nortikin/sverchok/pull/4323) in node data management. More than 50% of CPU resources can be wasted during using simple animation layouts with a lot of nodes. Also overhead of execution system and data management should be reduce to possible minimum. Second step is experimenting with multithreading. During the time when CPUs get more and more cores it looks logical step. Also node architecture and Sverchok vectorization system allows to apply this optimization to all nodes and only little changes are required from nodes side. Another way to go is to experiment with fast languages like C and C++ directly or via third party tools like Cython and Numba. It won't be easy to make all nodes to gain from using fast languages so most likely they can be applied only to bottleneck nodes.
- **UI**. There are thing to improve here. For example it would be nice to show last execution time of a tree somewhere. Also in case if a tree has many nodes it can be difficult to spot whether it has some nodes with errors so this information also could be shown. It would be nice to have some sort of node manager which can display list of nodes with some extra information about them like time execution or error massage. Such manager could sort nodes for example to find one with worst performance and to find its location. In case of big and slow trees it would be nice to have a progress bar of its evaluation to see how much work is done. There is no information about [nodes dependent on external libraries](https://github.com/nortikin/sverchok/issues/3410) in UI.
- **Nodes inconsistency**. One of the Sverchok problems is decentralized process of nodes developing. Each Sverchok developer has his own understanding of how nodes should work. So some similar nodes expect different data structure as input and have different data structure as output. Many nodes have different vectorization rules. All this make work with nodes hard and force to search some workarounds to prepare data for the input and handle output data. So some standard API for the nodes should be invented.
- **Node groups**. There is no way to debug geometry data now. Also it would be nice to support node viewers inside.

🙏 If you are interested in any of this features to be implemented you really can help by supporting me. Any income says that what I'm doing has a value for others. You can check my products dedicated to procedural modeling on [Blender market](https://blendermarket.com/creators/soluserg) and [Gumroad](https://app.gumroad.com/randum).

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
