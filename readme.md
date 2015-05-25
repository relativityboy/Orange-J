orange-j
version 3.0

Version 3.0 is a re-invention of orange-j's templating engine for the modern web. Syntax has been improved and clarified. 
A few features have been removed and replaced with others that do a better job EX:(no more inline functions, but you can 
develop your own tags for local or global use). Some formatters have been removed entirely as css and browsers have 
finally caught up.

The event system and validators have been dropped along with most of the basic utilities that accumulated in v2.x 
releases. With backbone, stickit, and backbone.validate they aren't needed. There *are* some utils and extensions that
may be included over time.


Development Roadmap:
1. tempate engine
  1. compile a simple template with {#}, {<attributeName>} and {<attributeName>[]}
2. test for template
3. lib manager
  1. add a template
  2. support helper functions
  2. support template inclusion
  3. templates become manager aware
  5. support inclusion of child templates
  6. support 'pathing' in template name in both template & manager
4. template engine - values
  1. supports getting value from parent
  2. supports absolute pathing
  3. supports relative pathing


** We want to include a global helper manager..**

When compiling templates - helper functions are searched for first.
If there are no helper functions registered with the given path, templates complain unless a global false property has 
been set for that.
