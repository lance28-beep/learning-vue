# Introduction
What is Vue.js
- A popular javascript framework for building user interfaces
- the core vue library is focused on doing one thing and doing that one thing really is building user interfaces
- Vue does not focus on the other aspects of your application like routing of HTTP requests
- vue has a rich eco system of other powerful libraries that you can intergrate.
- Vuex npm package for complex state management, Vue router for routing, vuetify for ui elements and a lot more.

Why Vue js?
- Vue currently has 175k Github stars - the third most starred Github repository in the world
- Thousands of developers around the world enjoy working with Vue.
- You are going to find solutions to most of the problems that you face.

* Vue is approachable.
- Familiarity with HTML, CSS and Javascript
- Add a script tag with a reference to vue.js and start building Vue applications
- Vue Devtools which gives insight into your apps.
- Vue CLI with which you can quickly scaffold and manage projects.
- Vue also has a component based architecture
- Vue is declarative
- Vue will make it painless for you to create complex user interfaces by abstracting away the difficult parts.

* Vue is versatile
- Create powerful single page applications from scratch using build tools like webpack.
- Incorporate Vue into your existing legacy projects and make progressive enhancement

* Vue is performant
- Vue measures just 20kb minified and gzipped at runtime
- Better performance because of virtual DOM


- Vue is a framework built by taking the good parts from a lot of other libraries and frameworks and then improving where necessary.
- Vue is going to be a great addition to you skill set.

Prerequisites:
- HTML, CSS and Javascript fundamentals
- ES6+ features
- A knowledge of modern javascript.


Four ways to add Vue
* CDN Package
><script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
* NPM
>npm install vue@next
- preferred approach over CDN when building large scale applications with Vue.
* Vue CLI
- Vue provides an official CLI for quickly scaffolding single page applications.
> npm install -g @vue/cli
> vue create <project-name>
* Vite
- An opinionated web dev build tool that serves your code via native ES Module imports.
- Your code is served at a lightning fast speed and you get nearly instant hot module replacement.
> npm init vite-app <project-name>

# Approach chosen for this series
CDN - incorporate Vue into a really old legacy code base or quickly prototype.
npm - is the recommended approach for building large scale applications with Vue.
Vue CLI - Takes only a few minutes to get up and running with hot reload, lint-on-save, and production-ready builds.
Vite -  its currently in the beta version

.Vue File
- A *.vue file is a custom file format that uses HTML-like syntax to describe a portion of the UI.
- Each *.vue file consist of three types of top-level language blocks.
> <template></template>
> <script></script>
> <style></style>