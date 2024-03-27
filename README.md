YAFF is a frontend library.

In reviewing all the other ones (which are great) we came to the conclusion that another was needed.
One were the intial page load is the fastest yet. One which you will never touch an html file again (html code...well, a little)

What we wanted was a full dynamic front end - independent of any backends, no curly braces, no special added on directives - just speed and functionality.
What we found was yet another front end.

We are proud to be introducing Yaff.js - a sleek, version 1.0 JavaScript frontend framework designed to simplify the use of content updates in your web applications. Yaff.js stands out by offering a straightforward approach to handling user interactions and data-driven updates, relying on the context of your html code to ensure quick and effortless coding, with great results.

**Core Features**
*Dynamic Event Listener Management*: Easily attach or remove event listeners to elements on your web page, supporting both direct element references and string IDs for element targeting.
*Seamless Data-Attribute Handling*: Utilize HTML data- attributes for element-specific actions, streamlining the process of associating elements with JavaScript behavior.
Effortless AJAX Calls: Fetch and display content without page reloads, thanks to built-in functions tailored for sending and receiving data, including form submissions and clicking actions.
Automatic Configuration Loading: Initialize your application with external configuration settings, allowing for flexible and scalable project setups.
Configuration and Setup
Yaff.js leverages a simple configuration mechanism loaded at runtime, enabling customization of API URLs and content update strategies. This configuration is fetched from a JSON file (/static/config.json), setting global parameters like apiUrl and innerOuter, which determine how content is fetched and where it's injected in the DOM.

Using Data- Elements
The power of Yaff.js lies in its ability to use data- attributes within your HTML to define interactive behaviors and data fetch operations:

Event Listeners: Add data- attributes to elements you wish to bind with event listeners. Yaff.js will automatically attach the specified event listeners, making your HTML cleaner and more semantic.
Content Updates: Specify which elements should fetch and display content dynamically through data- attributes. Yaff.js handles the rest, updating your UI in response to user actions without needing to write boilerplate AJAX code.
Getting Started
Define Your HTML Elements: Mark your interactive elements with *data-* attributes, indicating how they should interact with user actions and what content they should fetch or update.

<button id="loadButton" data-click="/api/loadMore">Load More</button>
<div id="contentArea" data-content></div>

Initialize Yaff.js: Ensure Yaff.js is loaded and initialized in your project. The framework will automatically attach event listeners based on your data- attributes and manage content updates.

<script src="path/to/yaff.js"></script>

Configure Your Application: Create a config.json file in the /static directory to define global settings like API URLs. Yaff.js will load these settings at startup, ensuring your application knows where to fetch data and how to handle content updates.
{
  "apiUrl": "https://example.com/api",
  "innerOuter": "inner"
}

Yaff.js offers a minimalist yet powerful approach to handling user interactions and dynamic content in web applications. By emphasizing simplicity, configurability, context-sensitivity and the use of html rather than special javascript operatoors, it enables developers to build interactive, data-driven websites with less code and greater clarity.
