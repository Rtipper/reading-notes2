# Class 7 Reading Notes - APIs Cont.

### APIs
- Roy Fielding: Helped write the first web servers, that sent documents across the Internet as well as did a ton of research explaining why the web works the way it does.
- The first things you type into a web browswer to access a specific site or loaction is called a protocol (i.e. http)
- Protocols are  capable of describing the location of something anywhere in the world from anywhere in the world and works as the foundation of the web (i.e. GPS coordinates)
- The whole world wide web is built on an architectural style called “REST”
- REST provides a definition of a “resource”, which is what those things point to.
- A web page is a “representation” of a resource, in turn -- Resources are just concepts (i.e. URLs)
- URLs tell the browser that there's a concept somewhere.
- A browser can then go ask for a specific representation of the concept -- specifically, the browser asks for the web page representation of the concept.
- In most cases, a resource has only a single representation.
- There's a bunch of new formats popping up all over the place.
- "Web Services" or "APIs" -- the basic concept is that machines could use the web just like people do.
- Computers can use those same protocols to send messages back and forth to each other.
- When Fielding and his buddies started building the web, being able to talk to any machine anywhere in the world was a primary concern.
- Most of the techniques we use at work to get computers to talk to each other didn't have those requirements.
- Some way of having one machine tell another machine about a resource that might be on yet another machine.
- "redirect"
- If everything that machines need to talk about has a corresponding URL, you've created the machine equivalent of a noun.
- Machines don't have a universal noun.
- Every programming language, database, or other kind of system has a different way of talking about nouns.
- Verbs are important.
- There's a powerful concept in programming and CS theory called “polymorphism” -- that's a geeky way of saying that different nouns can have the same verb applied to them.
- More or less, this is what engineers do in the web development world, thanks almost entirely to the popularity of RESTful web frameworks like Ruby on Rails.
- Just a few years ago, the large majority of developers were busy writing layers of complex specifications for how to access data in a different way that isn't nearly as useful or eloquent.
