## ECommerce Project

ECommerce provides a way to quickly get up and running with a fully configurable ECommerce site using Next.js.

Out of the box, the site uses completely static data coming from a provider at `providers/inventoryProvider.js`. You can update this provider to fetch data from any real API by changing the call in the `getInventory` function.

![Home](example-images/1.png)

### Getting started

1. Clone the project

```sh
$ git clone https://github.com/bladerunnersde/ecommerce.git
```

2. Install the dependencies:

```sh
$ yarn

# or

$ npm install
```

3. Run the project

```sh
$ npm run dev

# or to build

$ npm run build
```

## About the project

### Tailwind

This project is styled using Tailwind. To learn more how this works, check out the Tailwind documentation [here](https://tailwindcss.com/docs).

### Components

The main files, components, and images you may want to change / modify are:

**Logo** - public/logo.png  
**Button, ListItem, etc..** - components  
**Form components** - components/formComponents  
**Context (state)** - context/mainContext.js  
**Pages (admin, cart, checkout, index)** - pages  
**Templates (category view, single item view, inventory views)** - templates

### How it works

As it is set up, inventory is fetched from a local hard coded array of inventory items. This can easily be configured to instead be fetched from a remote source like Shopify or another CMS or data source by changing the inventory provider.

#### Configuring inventory provider

Update **utils/inventoryProvider.js** with your own inventory provider.
