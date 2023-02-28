# what is React-helmet.?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677341643593/e5c68bdd-4f92-491e-b392-16dcb1b50709.jpeg align="center")

`react-helmet` is a third-party library for React that allows you to manage the document head of your application. The document head is where you can define metadata, such as the title of your web page, character encoding, stylesheets, and JavaScript files. With `react-helmet`, you can dynamically update the document head based on the state of your application.

To use `react-helmet`, you need to install it first by running the following command in your terminal:

```plaintext
npm install --save react-helmet
```

Then, you can import it into your React component and use it to set the metadata in the document head. Here's an example:

```plaintext
import React from 'react';
import { Helmet } from 'react-helmet';

function MyComponent() {
  return (
    <div>
      <Helmet>
        <title>My Title</title>
        <meta name="description" content="My description" />
      </Helmet>
      <h1>Hello World</h1>
    </div>
  );
}
```

In this example, we're setting the title of the document to "My Title" and adding a meta tag with the name "description" and content "My description". These values will be updated in the document head whenever this component is rendered.

if you like my work then don’t forget to follow back I daily bring a new topic from this huge network and try to make it easy and clear to understand