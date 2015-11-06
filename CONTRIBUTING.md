Contributing to the Toolkit Documentation
===========================================

Anybody is welcome to contribute to the Toolkit Documentation!

Please review and follow the coding standards below. All submissions should be made as pull
requests. We recommend using a branch per pull request, and advise against making pull requests
based off your `master` branch. If you need assistance in creating a pull request, please ask
somebody via the Club Seiden [forum](http://club.alanseiden.com/community/forums/php-toolkit.3/) or [chat](http://club.alanseiden.com/community/pages/clubseidenchat/).

Documentation Standards
-----------------------

### GitHub-Flavored Markdown

Documentation is being written using [GitHub-flavored
Markdown](https://help.github.com/articles/github-flavored-markdown).

### Headings

Every file MUST contain a level 1 heading.

Level 1 headings MUST use the `====` format, with an equal number of `=` signs as the number of
characters in the preceding header line.

Level 2 headings MUST use the `----` format, with an equal number of `-` signs as the number of
characters in the preceding header line.

Level 3 and lower headings MUST use the `#` prefix, with one such character per level indicated.

### Line Length

Line lengths SHOULD be 100 characters or less; the only exception to this rule is when a URI on
the current line would push past the limit.

### Links

Links to other documents within the repository MUST be relative to the project root, not to the
current directory. For example, consider the following tree:

```
compatibility-wrapper/
    PCML.md
    error-reporting.md
```

If the file `compatibility-wrapper/PCML.md` links to the file `compatibility-wrapper/error-reporting.md`, the
following IS NOT correct:

```Markdown
[chapter on Error Reporting](error-reporting.md)
```

The following IS correct:

```Markdown
[chapter on Error Reporting](/compatibility-wrapper/error-reporting.md)
```

### Notes/Warnings/Etc.

Notes MUST be written using Markdown "blockquote" syntax:

```Markdown
> This is a note
```

GitHub-Flavored Markdown allows using markup inside blockquotes, including headers. We recommend
adding a header line at the appropriate header level when creating notes:

```Markdown
> ### Note about Notes
>
> This is a note about creating notes.
```

### File Names

File names MUST be enclosed in code tags ("\`\`"): `IbmiToolkit/Toolkit.php`, 'IbmiToolkit/ToolkitApi/CW/cwclasses.php',
etc.

### Lists

For consistency, unordered lists MUST use the `-` character to denote a list item; you MUST NOT use
the `*` character.

### Screencasts and Videos

We encourage the use of screencasts and videos for explaining concepts. However, you MUST NOT
include them in pull requests. Post them to public locations, such as [YouTube](http://youtube.com),
[Vimeo](http://vimeo.com), Google Drive, etc.; somewhere where they will likely persist. Then use
whatever HTML embed code they provide within your document in order to embed the video.