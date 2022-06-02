# Read 09

- The HTTP Request Lifecycle

- Step 1: Local Processing , Step 2 : Resolve an IP, Step 3 : Establish a TCP Connection, Step 4 : Send an HTTP Request , Step 5 :Tearing Down and Cleaning Up

- The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries. All the classes that we need are part of the java.net package.

- The disadvantages of using this method are that the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication.

- We can create an HttpUrlConnection instance using the openConnection() method of the URL class.

- If we want to add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance

- Adding headers to a request can be achieved by using the setRequestProperty() method: 

- To read the value of a header from a connection, we can use the getHeaderField() method: 

- HttpUrlConnection class allows setting the connect and read timeouts. These values define the interval of time to wait for the connection to the server to be established or data to be available for reading.

- The java.net package contains classes that ease working with cookies such as CookieManager and HttpCookie.

- We can enable or disable automatically following redirects for a specific connection by using the setInstanceFollowRedirects() method with true or false parameter:

-Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance. To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods

- If the request fails, trying to read the InputStream of the HttpUrlConnection instance won't work. Instead, we can consume the stream provided by HttpUrlConnection.getErrorStream().

- Note that the getFullResponse method will validate whether the request was successful or not in order to decide if it needs to use con.getInputStream() or con.getErrorStream() to retrieve the request's content.
