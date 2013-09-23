Grammar CMS
==========

Grammar CMS is not a CMS (yet), nor is it a content management framework. Rather, it is the idea of a CMS that I have been working on for years. It draws insipration from ideas in other content management systems such as ModX, Symphony CMS, Tumblr (yes, Tumblr), Pods Framework (for Wordpress), Django, and others.

The point here is not (yet) to build a content management system but to work out and design the developer and editorial workflow as well as define the schemas for its APIs, database entries, and settings.

## The Fundamentals
These are the core principles for Grammar CMS.
- **Designed for creators**: We keep touting that our websites providing great user experiences for the visitors, but treat our authors, editors, and designers as second class citizens. That will not happen here.
- **Create anywhere, publish everywhere (aka: API = not optional)**: It should not matter how the content comes in or goes out. 
- **Flexible data structures**: Not all websites are blogs, e-commerce sites, or collection of pages so stop building them as if they were.
- **Not everything is a page, but there *are* pages**: Some content makes sense as a part of a specific page and should be treated as such.
- **Customizable settings and semi-static content**: There are pieces of content which are static enough that it is inefficient to put them in a database, but shouldn’t require a developer to change.
- **No database abastractions**: The database structure should reflect the structure of its contents. If we cannot understand what the contents of the database is by just looking at it, we’ve failed our developer.
- **As many databases as needed and DB agnosticism**: Not all content makes sense in a relational database, instead, the CMS should merely define a good standard schema and let the developer decide what is best to use and how many.
- **Databases are for data, not settings**: All settings and customizations should reside as static content in the file structure.
- **Built for git and git submodules**: Not only should customizations (such as extensions) live in the file structure, but they should also live together so you only need to use a single `git submodule add` command to add all the necessary customizations to duplicate your project into a blank install.
- **Version control everything**: All content should be versioned to help the editorial process.
- **Flexible I/O**: No matter the output—HTML, XML, JSON, carrier pidgeon—developers should be able to define how content comes in and goes out.
- **Export content = also not optional**: Figuring out how to export content because you need to move on should never involve hours of searching on Google.
- **Granular permissions**: Content creation is not a democracy, not all users are equal, and not all websites are alike.
- **Flexible admin with smart defaults**: The CMS should not be a mess of features and settings. Features and advanced settings should be compartimentalized to offer what users need to do and let them do it with as little distraction as possible. However, the admin console should be as customizable as its data structures.
- **Good browser-based tools**: We prefer our own dev tools, but sometimes we just want to get in, make a change, and get out.

## Inspiration
- Customized page content in [ModX](http://modx.com/)
- [Sections in Symphony CMS](http://www.getsymphony.com/learn/concepts/view/sections/) and [Pods Framework](http://pods.io/)
- Customized creation process per-post type on Tumblr
