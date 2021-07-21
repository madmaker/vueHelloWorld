# Vue Hello World

According to Vue Handbook:

https://flaviocopes.nyc3.digitaloceanspaces.com/vue-handbook/vue-handbook.pdf

## First example
First I'll use the most basic example of using Vue. You create an HTML file which contains

```html 
<html>
  <body>
    <div id="example">
      <p>{{ hello }}</p>
    </div>
    <script src="https://unpkg.com/vue"></script>
    <script>
        new Vue({
            el: '#example',
            data: { hello: 'Hello World!' }
        })
    </script>
  </body>
</html>
```
              9

 and you open it in the browser. That's your first Vue app! The page should show a "Hello World!" message.

I put the script tags at the end of the body so that they are executed in order after the DOM is loaded.

What this code does is, we instantiate a new Vue app, linked to the #example element as its template (it's defined using a CSS selector usually, but you can also pass in an HTMLElement).

Then, it associates that template to the data object. That is a special object that hosts the data we want Vue to render.

In the template, the special {{ }} tag indicates that's some part of the template that's dynamic, and its content should be looked up in the Vue app data.


## Run project

Open package.json and run script 'start' (in phpstorm just click "run" button on left side)

Then open http://localhost:5000     in your browser