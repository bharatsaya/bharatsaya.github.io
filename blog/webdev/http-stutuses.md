---
title: HTTP Status Codes
layout: default
permalink: /blog/http-status-codes
nav_exclude: true
---

# HTTP Status Codes

So, when you see the infamous 404 Not Found or the whimsical 418 I'm a teapot (See https://www.google.com/teapot if you've never seen it before), you know you're dealing with the world of web. When you're in the web, and you need to communicate with other players in the field - like a browser talking to a server or a service calling another API endpoint - HTTP Status Codes come into play. They tell us how things are going - good bad or ugly. 


> ### HTTP Status codes are three digit numbers and they're grouped into five categories - 
>
> - 1xx - These are used for informational purposes, and rare because they're not used in RESTful APIs    
> -  2xx - All A-OK.These are the happy ones. The dopamine of the web. If there you never got a 2xx, you'd not feel like doing anything online, right? 
> - 3xx - Wait, you need to go somewhere else. Redirection!
> - 4xx - I'm telling you it's all your fault! Just as common in the real world as it is in the web world
> - 5xx - Oops, something went wrong. The server knows something is wrong and has the humility to accept it.

Finally, if a server doesn't respond at all, usually the client throws a "Timed Out" exception but this is not an HTTP Status code rather something that happens at the client end because in this case the server is not feeling like talking, right?

---

Now, let's look at some of the more commonly used ones

- 200 OK
    The request was successful, and the response body contains the requested resource.

- 201 Created
    The request was successful, and a new resource was created as a result.

- 204 No Content
    The request was successful, but there's nothing to return (i.e., the response is empty).

- 301 Moved Permanently
    The URI of the requested resource has been changed permanently. The new URI is provided in the response.

- 302 Found
    This response code means that the URI of requested resource has been changed temporarily.

- 400 Bad Request
    The server could not understand the request due to some kind of error in the client's request.

- 401 Unauthorized
    The client must authenticate itself to get the requested response.

- 403 Forbidden
    The client does not have access rights to the content; that’s why the server is refusing to give proper response.

- 404 Not Found
    The server can not find the requested resource.

- 429 Too Many Requests
    The access to server is "rate limited" based on your subscription or access level. 

-   500 Internal Server Error
    The server has encountered a situation and, unfortunately, it doesn't know how to handle.

---

But there are many more out there but like the 80/20 rule, these 20 percent cover the 80 percent of the practical use cases. 2xx.