To provide data to an HTML page as parameters in the link that opens the page, you can use query parameters in the URL. Query parameters allow you to pass data to the HTML page in the form of key-value pairs. Here's an example:

Let's say you have an HTML page called "example.html" and you want to pass two parameters, "name" and "age", with respective values "John" and "25". You can construct the link as follows:

<a href="example.html?name=John&age=25">Open Example</a>
When the user clicks on the link, it will open the "example.html" page, and the parameters will be accessible in the page's URL. To retrieve these parameters using JavaScript, you can use the URLSearchParams API.

Here's an example of how you can retrieve the parameters in "example.html" using JavaScript:
<script>
  const urlParams = new URLSearchParams(window.location.search);
  const name = urlParams.get('name');
  const age = urlParams.get('age');
  
  console.log(`Name: ${name}`);
  console.log(`Age: ${age}`);
</script>

