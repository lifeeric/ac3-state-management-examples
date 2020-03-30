<h2 align="center">Apollo Client 3 State Management Examples</h2>

<p align="center">Learn how to use AC3 for local and remote state management</p>

## About

[Apollo Client 3](https://www.apollographql.com/docs/react/v3.0-beta/migrating/apollo-client-3-migration/) is a state management library that enables you to work with remote GraphQL data. Apollo Client handles all of the data fetching logic for you- all you have to do is write the queries and mutations, and you're good to go.

We have found that it can be challenging for developers coming from another state management library (like [Redux](https://redux.js.org/)) to fully grasp the AC3-way of doing things.

### What we're building

This repo contains several versions of the same Todo app, both Apollo Client and Redux examples, to demonstrate best practices on using Apollo Client to build applications using solely **local state** in addition to the real-world **remote state** use case.

![](https://user-images.githubusercontent.com/6892666/76266873-4cd96a00-623f-11ea-8367-e0735d63a54f.png)

## Examples

### Apollo Local State Example

> Summary: Using Apollo Client 3's **Reactive Variables API** (docs/blog post coming soon), we can store the entire application state locally (and optionally persist it using local storage).

[Check out the local state example](https://github.com/apollographql/ac3-state-management-examples/tree/master/apollo-local-state).

### Apollo Remote State Example

> Summary: Hooking Apollo Client up to a remote GraphQL API, the client-side cache is smart enough to automatically update the cache after _most_ mutations successfully complete. For mutations that perform interactions against arrays or have additional client-side side-effects, we can help the cache decide what to do next by writing our update logic in the `useMutation`'s `update` function.

[Check out the remote state example](https://github.com/apollographql/ac3-state-management-examples/tree/master/apollo-remote-state)

### Redux Local State Example

> Summary: The Redux architecture provides us with a well-defined mental model for how to update state in an immutable way. We've provided this example in order to compare how to accomplish the same tasks in AC3 and in Redux.

[Check out the local state (with Redux) example](https://github.com/apollographql/ac3-state-management-examples/tree/master/redux-local-state)
 
