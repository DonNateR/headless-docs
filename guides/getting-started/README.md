# Getting Started Guide

In this guide, you'll learn the basics of deploying apps on the WP Engine Headless Platform.

Requirements:

- [Node.js](https://nodejs.org/en/download/)
- [Git](https://git-scm.com/downloads)
- WP Engine Headless CLI tool ([install](/#installation))

What we'll cover:

- [Supported apps](#supported-apps)
- [Creating your first app](/guides/getting-started/create-app)
- [Deploying your first app](/guides/getting-started/deploy-app)
- [Making changes to your app (dev workflow)](/guides/getting-started/workflow)

## Supported Apps

The platform supports [Node.js](https://nodejs.org/)-based applications.

Node.js uses npm for its package management, which allows you to set the version of Node your applications require via the `engines` property inside your project's `package.json`.

```json
{
  "engines": {
    "node": "12.18.0"
  }
}
```

The supported versions of Node are 10, 12, and 14. Specifying a version of Node below the minimum supported version will result in the application of the minimum supported version (10); specifying a higher version will result in the application of the maximum supported version (14).
