ElasticUI
=========

ElasticUI is a set of AngularJS directives making it easy to rapidly build a frontend on top of Elasticsearch. It builds upon the elastic.js implementation of the Elasticsearch DSL.

**The concept of ElasticUI is to have one "view" of your index to which you can add aggregations, sorting, paging, filters by adding directives in your html.**

Getting started (demo file)
---
The easiest way to get started is to checkout the [demo file][3]. This file demonstrates a simple use of facets, search and pagination. Just change 4 fields in the source to match your Elasticsearch setup and mapping.

[Read more about the widgets used in the demo][4].

Creating a project from scratch
---
Add the following files to your Angular project:
 - elasticui.js from dist/
 - elastic.js from [fullscale/elastic.js][1]
 - elasticsearch.angular.js from [elasticsearch.org][2]

Set up ElasticUI in your project by defining your ElasticSearch host as *euiHost*:

    angular.module('yourApp', ['elasticui']).constant('euiHost', 'http://localhost:9200');

Set the `eui-index="INDEX_NAME"` on the `<body>` tag, now you can get started adding ElasticUI components to your view (see below).

Components
===
The directives you can use for aggregations (facets), sorting, paging and filtering your view are documented in [docs/components.md][5]

Screenshot
===
Example dashboard built on top of this project:

![World Cup Twitter Dashboard](https://raw.githubusercontent.com/YousefED/ElasticUI/master/docs/example_twitter_dashboard.png)



  [1]: http://github.com/fullscale/elastic.js
  [2]: http://www.elasticsearch.org/guide/en/elasticsearch/client/javascript-api/current/browser-builds.html
  [3]: https://github.com/YousefED/ElasticUI/blob/master/examples/demo/demo.html
  [4]: https://github.com/YousefED/ElasticUI/blob/master/docs/widgets.md
  [5]: https://github.com/YousefED/ElasticUI/blob/master/docs/components.md
