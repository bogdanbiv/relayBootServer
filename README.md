# Relay Boot Server

Most React/Relay apps have similar server requirements - this is an attempt to bootstrap such a server

This kit includes an app server, a GraphQL server, and a transpiler that you can use to get started building an app with Relay. For a walkthrough, see the [Relay tutorial](https://facebook.github.io/relay/docs/tutorial.html).

## Project Plan

0. Start with Relay Starter Kit
  * npm install
  * smoke tests

1. [Verify Webpack/React Transform features](../../issues/1)
  * Simple React Component is rendered
  * JSX transform
  * Hot Module Reload
  * Red Error flasher
  * ES2015 support on the client

2. Verify GraphQL features
  * seed database / backend/s
  * Graffiti based schema
  * extend schema with REST backend/s

3. Change webserver to Koa, add Lusca for security
  * port middleware to use generators
  * check http2 support in NodeJS (also check Webpack for compat)
  * TLS encryption
  * Detect connection performance (server ?)

4. Logging & monitoring
  * bunyan
  * weston

5. Authentication & Authorization:
  * One approach to authentication/authorization with GraphQL-based server - https://github.com/mostr/graphql-auth
  * Limit introspection capability programatically - https://github.com/graphql/graphql-js/issues/113

6. Test suite
  * Unit test components
  * Component integration
  * Mocha, Chai, Sinon
  * WebDriver ?
  * Karma (other runners ?)

7. Task runner
  * Gulp / Slush
  * Fly / Flightplan
  * Deployment task
  * Generate static site via React (server side) - during idle time
  * Re/Generate schema (data/schema.json) and restart server
  * Seed database

8. Cluster support
  * Geo-optimisation ?
  * latency ?

9. React tools
  * GraphiQL
  * Playground
  * Block editors (Structor, Kattappa, Colonel Kurtz)

## License

Relay Starter Kit is [BSD licensed](./LICENSE). We also provide an additional [patent grant](./PATENTS).

1043    
-----
