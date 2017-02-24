<p align="center">
  <img src="https://union.io/images/repo/20170224-01--fda070.png" width="750">
</p>

<h1 align="center">
Technical Writing Style Guide
</h1>

Independent Tech Writers Co. strives for a consistent and high quality style of technical writing throughout its entire body of work. Here are the formal standards and best practices for all pull requests initiated by the technical writers working with ITW Co.

## Table of Contents

1. [General Writing](#general-writing)
1. [Additional Standards](#additional-standards)
1. [Code & Comments](#code--comments)
1. [Commit Messages](#commit-messages)
1. [Writing for User Interfaces](#writing-for-user-interfaces)

## General Writing

When editing README files and other long-form documentation, be sure to follow all commonly accepted rules of grammar, punctuation and spelling. Spellcheck _everything_. Try to be concise without being terse: A README file provides the voice & tone for the entire codebase and should work to ensure the code is the center of attention, not the documentation.

Use the [Economist Style Guide](http://www.economist.com/styleguide) as a general guideline for writing in English. Although its intended audience is the journalism community, it also provides a useful starting point for technical writing.

Here are some important points to follow from the _Economist_ guide.

<a name="general-writing--dates"></a><a name="1.1"></a>
- [1.1](#general-writing--dates) **Dates**: Dates are month, day, year — no dashes. For date ranges, use a single hyphen with no spaces.

	**Good**:
	```
July 20th 2003. Monday July 9th. July 4th-8th 1776.
	```

	**Bad**:
	```
July 20, 2003. Monday, July 9. July 4th - 8th.
	```

<a name="general-writing--numerals"></a><a name="1.2"></a>
- [1.2](#general-writing--numerals)  **Numerals**: Try to spell all numbers zero through nine — unless it looks strange — but always use numerals at 10 and above (until you reach thousands, millions, billions, etc).

	**Good**:
	```
Take five minutes. Hold the third note. One in a million.
	```

	**Bad**:
	```
Take 5 minutes. Hold the 3rd note. 1 in a million.
	```

<a name="general-writing--parentheses"></a><a name="1.3"></a>
- [1.3](#general-writing--parentheses)  **Periods within parentheses**: Don't use periods within parentheses or brackets unless they include one or more full sentences.

	**Good**:
	```
This should feel natural (like a logical next step).
Perfect! (That was indeed our intent.)
	```

	**Bad**:
	```
This should feel natural (like a logical next step.)
Perfect! (That was our intent).
	```

<a name="general-writing--abbreviations"></a><a name="1.4"></a>
- [1.4](#general-writing--abbreviations)  **No periods in abbreviations or titles**

	**Good**:
	```
The USA
JP Morgan
Mr and Mrs Smith
	```

	**Bad**:
	```
The U.S.A.
J.P. Morgan
Mr. and Mrs. Smith
	```

<a name="general-writing--oxford-comma"></a><a name="1.5"></a>
- [1.5](#general-writing--oxford-comma)  **Sorry, no Oxford comma**: Although contentious, we recommend the _Economist_ method: no Oxford comma unless the sentence would become unclear otherwise.

	**Good**:
	```
Please update your repository, packages and modules.
	```

	**Not-so-good**:
	```
Please update your repository, packages, and modules.
	```

**[⬆ back to top](#table-of-contents)**

## Additional Standards

The _Economist_ guide wasn't written with Markdown in mind, so here are some additional rules to follow when editing documentation:

<a name="additional-standards--markdown"></a><a name="2.1"></a>
- [2.1](#additional-standards--markdown) **Use markdown whenever you can**: Markdown is well-supported and degrades fairly well. When editing a README file, or any in-codebase documentation, use Markdown unless the project requires otherwise.

	Use the [GitHub Markdown standard](https://guides.github.com/features/mastering-markdown/) — it's easy to learn, flexible and mature. Use a Markdown editor, like [MacDown](https://macdown.uranusjr.com/) (for Mac), to ensure your Markdown code works before committing it.

<a name="additional-standards--list-items"></a><a name="2.2"></a>
- [2.2](#additional-standards--list-items) **List items**: Use Markdown list items liberally. And be sure to use a period only if the list item contains two or more full sentences. Otherwise, no period.

	**Good**:
	```
- Update README file
- Fix any parsing bugs
- Rename the repository. The joke's not funny anymore.
	```

	**Bad**:
	```
- Update README file.
- Fix any parsing bugs.
- Rename the repository. The joke's not funny anymore.
	```

<a name="additional-standards--ellipsis"></a><a name="2.3"></a>
- [2.3](#additional-standards--ellipsis) **Use periods for ellipses**: When writing an ellipsis, don't use the actual ellipsis character (…, which is _option+;_ on a Mac keyboard, and the `&hellip;` HTML entity), even though it is technically the proper one to use. Just use three consecutive periods (...) since most future editors will write it that way.

<a name="additional-standards--apostophes"></a><a name="2.4"></a>
- [2.4](#additional-standards--apostophes) **Don't use curly-quotes for apostophes or quotation marks**: Use prime marks (' and ") instead of proper quotation marks (‘’ and “”). The "proper" way to write an apostophe is technically with the curly quotation mark (’, which is the HTML symbol `&rsquo;`). However, it's much more common in daily communication to use the prime mark ('), which is what is on a standard English-language keyboard. So, when contributing to a shared project, just use the prime mark to ensure future editors don't introduce inconsistencies. This also goes for double-quotes (use "" instead of “”).

	**Good**:
	```
- There aren't any other options!
- We are not a "traditional startup".
	```

	**Bad**:
	```
- There aren’t any other options!
- We are not a “traditional startup”.
	```

**[⬆ back to top](#table-of-contents)**

## Code & Comments

Contributing code should always be done in accordance with the contribution guidelines and standards already in place for the project you’re contributing to. Defer to the project precedents for everything from tabs-vs-spaces to naming conventions. When in doubt, use well-respected style guides for the particular programming language (like the [AirBnB JavaScript Style Guide](https://github.com/airbnb/javascript) for JavaScript and JS-like languages, for example).

Code _commenting_, however, can be fairly standard. Follow these rules.

<a name="code--comments--capitalize"></a><a name="3.1"></a>
- [3.1](#code--comments--capitalize) **Capitalize consistently**: Capitalize traditionally, with the first letter of a comment always being capitalized (unless it's a special variable or keyword, of course).

	```
// This is a good comment

// So is this one

// this isn't a good comment, however
	```

<a name="code--comments--periods"></a><a name="3.2"></a>
- [3.2](#code--comments--periods) **Do not end single-sentence comments with periods**: Capitalize traditionally, with the first letter of a comment always being capitalized (unless it's a special variable, for example).


	```
// Good: A good one-sentence comment has no ending period

// Also good: Periods are required here. This comment has two sentences.

// Bad: A one-sentence comment with a period.
	```


<a name="code--comments--empty-lines"></a><a name="3.3"></a>
- [3.3](#code--comments--empty-lines) **Empty lines**: A comment line descibing the next line of code should have an empty line above it, and no empty line below it.

	**Good**:
	```
var text = someLineOfCode();

// Ensure the text is formatted properly
text = text.formatProperly();
	```

	**Bad**:

	```
var text = someLineOfCode();
// Ensure the text is formatted properly
text = text.formatProperly();
	```

	**Also bad**:
	```
var text = someLineOfCode();

// Ensure the text is formatted properly

text = text.formatProperly();
	```

<a name="code--comments--sequence"></a><a name="3.4"></a>
- [3.4](#code--comments--sequence) **Avoid sequential phrasing**: Code comments shouldn't be "stateful"; that is, they shouldn't rely on _comment Y_ always following _comment X_. To that end, avoid using sequential phrasing, like "first", "then" or "after that".

	**Good**:
	```
// Assign the function output to a variable
var text = someLineOfCode();

// Ensure the text is formatted properly
text = text.formatProperly();

// Return the text
return text;
	```

	**Bad**:
	```
// First, assign the function output to a variable
var text = someLineOfCode();

// After that, ensure the text is formatted properly
text = text.formatProperly();

// Finally, return the text
return text;
	```

<a name="code--comments--apostrophes"></a><a name="3.5"></a>
- [3.5](#code--comments--apostrophes) **Use prime marks for apostophes**: As mentioned in [#2.4](2.4), do not use curly-quotes (‘’ or “”) for apostrophes or quotation marks. Use prime marks (' and ") instead.

<a name="code--comments--end-of-line"></a><a name="3.6"></a>
- [3.6](#code--comments--end-of-line) **Avoid commenting at the end of a line of code**: Ideally, comments belong on a line of their own. Only put them at the end of a line of code if you must (like in the rare situation that you must comment on just one item in a large array). Always try to avoid this if possible, however.

	**Good**:
	```
// Truncate the string at 35 characters
$string.truncate(35);
	```

	**Bad**:
	```
$string.truncate(35); // Truncate the string at 35 characters
	```

	**Possible exception to this rule:**
	```
var myArray = {
	'orgeat',
	'passionfruit',
	'honeySyrup',    // This must be camel-cased!
	'falernum',
	'gin',
	'rum',
	'lime'
}
	```

<a name="code--comments--line-width"></a><a name="3.7"></a>
- [3.7](#code--comments--line-width) **Be thoughtful with line length**: When a comment line length is going to exceed the column width specified for a project, break the comment into multiple lines. How you do this will depend on the programming language. If the project hasn't specified a column width, break at about 100 characters.

	**Good**:
	```
/**
* I'd just like to interject for a moment. What you're referring
* to as Linux, is in fact, GNU/Linux, or as I've recently taken
* to calling it, GNU plus Linux.
**/
	```

	**Bad**:
	```
// I'd just like to interject for a moment. What you're referring to as Linux, is in fact, GNU/Linux, or as I've recently taken to calling it, GNU plus Linux.
	```

**[⬆ back to top](#table-of-contents)**

## Commit Messages

Commit messages are generally only meant to be read by developers and those with technical knowledge of a project. This means writing style is more flexible here, since it won't reflect on the voice & tone of the project as a whole.

Always be sure to follow any commit formatting rules enforced by the project. Some projects, like the Linux kernel, will reject any pull request out-of-hand for even a small deviation from the commit template. **Never compromise your work by neglecting to follow a direction.**

For projects without strict commit standards: Try your best to describe your commit entirely within the commit message summary. This is a maximum of 50 characters, so there's no room for extended descriptions. If you absolutely must give more information, give a descriptive summary of less than 50 characters, then be as straightfoward as possible in the extended description. Follow the code-commenting rules as described above.

<a name="commit-messages--voice"></a><a name="4.1"></a>
- [4.1](#commit-messages--voice) **Always use the second-person voice when writing a commit summary**: Write your summary in the present-tense, as if it were a verbal command you could apply to the codebase.

	**Good**:
	```
$ git commit -am "Update the README with examples"
	```

	**Bad**:
	```
$ git commit -am "Updated the README with examples"
	```

	**Bad**:
	```
$ git commit -am "Updating the README with examples"
	```

<a name="commit-messages--capitalize"></a><a name="4.2"></a>
- [4.2](#commit-messages--capitalize) **Capitalize your commits**: Capitalize each sentence in your commit summary (although in truth you should rarely have more than one sentence).

<a name="commit-messages--periods"></a><a name="4.3"></a>
- [4.3](#commit-messages--periods) **Don't use periods for single-sentence commits**: Follow the same rules as code commenting above. If your summary is just one sentence, don't put a period at the end of it. If it's more than one sentence (although, again, this is very rare) use periods at the end of each sentence.

**[⬆ back to top](#table-of-contents)**

## Writing for User Interfaces

Writing for users is best left to the project maintainers and their copywriting team, since it needs to reflect the precise voice & tone the software and brand aims to create. However, if asked to edit messaging for user interfaces, use Google's [style guide for UI writing](https://material.io/guidelines/style/writing.html) as your guide. It's an indispensable tool for messaging within an interface.

Note that this means some rules in this guide, like the ones regarding apostrophes, must be superseded. Here are just a few of the important points to note from Google's guide.

<a name="writing-for-user-interfaces--focus"></a><a name="5.1"></a>
- [5.1](#writing-for-user-interfaces--focus) **Be friendly, respectful, and focus on the user**: Your app's text should complement its design: intuitive, efficient, casual, and trustworthy.

	**Good**:
	```
MyApp isn’t responding
-- Do you want to close it?
	```

	**Bad**:
	```
Sorry!
-- Activity in MyAppActivity (in the MyApp app) is not responding
	```


<a name="writing-for-user-interfaces--positive"></a><a name="5.2"></a>
- [5.2](#writing-for-user-interfaces--positive) **Be positive**: Present information in a positive light. It's reassuring.

	**Good**:
	```
Use 24 characters or fewer for file names
	```

	**Bad**:
	```
Your file name must be less than 25 characters
	```

<a name="writing-for-user-interfaces--essential"></a><a name="5.3"></a>
- [5.3](#writing-for-user-interfaces--essential) **Be essential**: Communicate essential details, so that users can focus on their own tasks. Sometimes the most effective UI contains no text at all.

	**Good**:
	```
Your phone is contacting Google. This can take up to five minutes.
	```

	**Bad**:
	```
Your phone needs to communicate with Google servers to sign in to your account. This may take up to five minutes.
	```

**[⬆ back to top](#table-of-contents)**

## Contributing

Please feel free to contribute to this guide. Pull requests that follow the rules outlined in this document are happily accepted.
