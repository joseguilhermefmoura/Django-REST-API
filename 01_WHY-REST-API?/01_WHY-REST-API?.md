# Why REST API?

A Rest API is a standardized way to provide data to other applications. Those applications can then use the data however they want. Sometimes, APIs also offer a way to other applications to make changes to the data.

There are a few <u>key options</u> for a REST API request:

- **GET** — The most common option, returns some data from the API based on the endpoint (URI) you visit and the parameters you provide.
- **POST** — It creates a new record that gets appended to the database.
- **PUT** — Looks for a record at the given URI you provide. If it exists, update the existing record. If not, create a new record.
- **DELETE** — Deletes the record at the given URI.
- **PATCH** — Update individual fields of a record.

Typically, <mark> an API is a window into a database.</mark> The API backend handles querying the database and formatting the response. What you receive is a static response, usually in <strong>JSON</strong> format, of whatever resource you requested.

REST APIs are so commonplace in software development, it's an essencial skill for a developer to know how they work. APIs are how applications communicate with one another or even whithin themselves.

So, let's think about an REST API this way:

DJANGO ORM creates & manages database models & queries, then DJANGO serves React as a collection of static files when someone visits a URL, then React can GET, POST, etc data from the database via the REST API. So, the Django Rest Framework serializes data from the Django ORM and allow access/updates via a RESTful API.

That's what the image below represents:

![Picture representing what was said above.](https://github.com/joseguilhermefmoura/Django-REST-API/blob/main/1.png?raw=true)

That is: <mark>in web development, many applications rely on REST APIs to allow the front end to talk to the back end.</mark> If you're deploying a React application atop Django, for instance, you'll need an API to allow React to consume information from the database.

<mark>The process of querying and converting tabular values into JSON or another format is called **serialization**.</mark> When you're creating an API, correct serialization of data is the major challenge. 