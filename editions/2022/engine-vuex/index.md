---
title: 'WWT 2022 Release Notes: Vue/Vuex Engine Interface'
nav_exclude: true
---

# WWT 2022 Release Notes: Vue/Vuex Engine Interface

WWT 2022 marks the first release of [@wwtelescope/engine-vuex][npm], a
[TypeScript] package providing managed access to [the WWT WebGL
engine](../engine/) in the [Vue.js] framework using the [Vuex] state management
system.

[npm]: https://www.npmjs.com/package/@wwtelescope/engine-vuex/
[TypeScript]: https://typescriptlang.org/
[Vue.js]: https://vuejs.org/
[Vuex]: https://vuex.vuejs.org/

The WWT rendering engine is an extremely complex system that maintains a huge
amount of internal state. It can be **very** challenging to try to build an
interface that properly reacts to the wide variety of modes that the engine can
reach. It doesn’t help matters that the engine implementation often results in
very non-idiomatic JavaScript APIs.

The [@wwtelescope/engine-vuex][npm] package tackles this challenge by wrapping
up all of the engine’s funkiness inside the tried-and-true state management
system of the Vue/Vuex combination. While the interface layer cannot make the
complexity go away, it makes it massively easier to handle. The official WWT
[embed](../embed/) and [research](../research-app/) web apps are built on this
package.

See [the API documentation][apidocs] to learn more about the module’s usage. See
the [detailed WWT 2022 components list](../components/) for links to developer
resources such as code repositories and changelogs.

[apidocs]: https://docs.worldwidetelescope.org/webgl-reference/latest/apiref/engine-vuex/

[Go back to the WWT 2022 edition notes.](..)
