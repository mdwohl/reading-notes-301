### Class 13 Reading
## Update/Delete

What happens to data when forms are submitted?

A *client* (usually the browser) sends a request to a *server*, which is most often a web server. This is sent via HTTP protocol -- the same protocol is used for sending and answering the request. The actual browser form is just a slick way of gathering input to make that HTTP request.

All of the attributes of the form element allow the dev to configure how the req is sent. Most important are the action and method attributes.

**Action** defines *where* the data gets sent -- it must have a valid URL value (absolute or relative). It defaults in absence of a URL to the page that contains the form. The name and value of the form are sent in the form of name=value. Action's value should be a serverside file that can validate and handle the incoming data. Precisely *how* the data is sent depends on **method**.

**Method** defines which way data is sent -- HTTP protocol provides us with several options for a request. The most common methods are GET and POST. Each contains a header that contains metadata and body that can contain information that helps the server process the request.

**Get** method is used on the client side to ask the server to send back resource x. The browser sends an empty body, which appends this data to the URL in the form of name/value pairs.

**Post** is how the browser talks to the server when it needs a response that accounts for the data from the HTTP request body -- when the server's response needs to be appropriate relative to the data send by the request. A big difference is that the data is not appended to the URL.

HTTP requests are not displayed to the user, but can be seen in dev tools. There are multiple languages and frameworks that can be used to handle forms on the server side.