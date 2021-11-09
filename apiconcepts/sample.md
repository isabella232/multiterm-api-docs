# Sample

## [Connecting to a MultiTerm Server](connect.md)
The first thing you need to do before you can access MultiTerm client functionality programmatically is to initiate a MultiTerm client object instance, i.e.:
## [Selecting a Termbase](termbase.md)
## [Searching a Termbase](searching.md)
The TermbaseSearch class allows you to programmatically perform a search in a particular termbase. When searching a termbase you need to provide a number of parameters such as the search term, the search index, the maximum number of terms that the search should yield, etc.
## [Retrieving Entry Content](entry.md)
MultiTerm entries are physically stored as XML blobs in the database backend. Retrieving an entry basically involves retrieving the XML content from the database. Once you have retrieved the content of an entry, you can, for example, parse it using the DOM API, apply an XSL stylesheet to it for transformation, etc.
## [Adding new Entries](adding.md)
To add new entries to a termbase, you first need to 'construct' the entry XML content to store in the termbase.
## [Sample Application in VBA](sample_vba.md)
Using Visual Basic you can integrate MultiTerm functionality into applications such as Microsoft Office or any other application that supports VBA (Visual Basic for Applications).
## [XML Schema: MTF]()
This schema describes the following elements and attributes:
## [XSD schema: MTF source](xsd_schema.md)