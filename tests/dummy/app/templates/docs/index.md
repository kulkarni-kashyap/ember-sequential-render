
Modern SPA layouts have an overload of information in the user's viewport in any given route. What's preventing secondary information from blocking or taking up resources, which, if left alone, would drastically improve the rendering of the primary content? 
[More thoughts on Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path)

ember-sequential-render helps in CRP optimization with the following features:

### Prioritized Sequential Rendering

A composable container component, **sequential-render**, which prioritizes and queues the data fetch and the rendering of its content with the necessary loading states.

### Postrender callback

An elegant way to defer the load of thirdparty resources after the rendering of the highest priority item in your queue.