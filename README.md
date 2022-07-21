# centuryblogs.github.io

Markdown	HTML	Rendered Output
# Heading level 1	<h1>Heading level 1</h1>	
Heading level 1
## Heading level 2	<h2>Heading level 2</h2>	
Heading level 2
### Heading level 3	<h3>Heading level 3</h3>	
Heading level 3
#### Heading level 4	<h4>Heading level 4</h4>	
Heading level 4
##### Heading level 5	<h5>Heading level 5</h5>	
Heading level 5
###### Heading level 6	<h6>Heading level 6</h6>	
Heading level 6
Alternate Syntax
Alternatively, on the line below the text, add any number of == characters for heading level 1 or -- characters for heading level 2.

Markdown	HTML	Rendered Output
Heading level 1
===============	<h1>Heading level 1</h1>	
Heading level 1
Heading level 2
---------------	<h2>Heading level 2</h2>	
Heading level 2
Heading Best Practices
Markdown applications don’t agree on how to handle a missing space between the number signs (#) and the heading name. For compatibility, always put a space between the number signs and the heading name.

✅  Do this	❌  Don't do this
# Here's a Heading

#Here's a Heading
You should also put blank lines before and after a heading for compatibility.

✅  Do this	❌  Don't do this
Try to put a blank line before...

# Heading

...and after a heading.	Without blank lines, this might not look right.
# Heading
Don't do this!
Paragraphs
To create paragraphs, use a blank line to separate one or more lines of text.

Markdown	HTML	Rendered Output
I really like using Markdown.

I think I'll use it to format all of my documents from now on.	<p>I really like using Markdown.</p>

<p>I think I'll use it to format all of my documents from now on.</p>	
I really like using Markdown.

I think I'll use it to format all of my documents from now on.

Paragraph Best Practices
Unless the paragraph is in a list, don’t indent paragraphs with spaces or tabs.

 Note: If you need to indent paragraphs in the output, see the section on how to indent (tab).
✅  Do this	❌  Don't do this
Don't put tabs or spaces in front of your paragraphs.

Keep lines left-aligned like this.

    This can result in unexpected formatting problems.

  Don't add tabs or spaces in front of paragraphs.
Line Breaks
To create a line break or new line (<br>), end a line with two or more spaces, and then type return.

Markdown	HTML	Rendered Output
This is the first line.  
And this is the second line.	<p>This is the first line.<br>
And this is the second line.</p>	
This is the first line.
And this is the second line.

Line Break Best Practices
You can use two or more spaces (commonly referred to as “trailing whitespace”) for line breaks in nearly every Markdown application, but it’s controversial. It’s hard to see trailing whitespace in an editor, and many people accidentally or intentionally put two spaces after every sentence. For this reason, you may want to use something other than trailing whitespace for line breaks. If your Markdown application supports HTML, you can use the <br> HTML tag.

For compatibility, use trailing white space or the <br> HTML tag at the end of the line.

There are two other options I don’t recommend using. CommonMark and a few other lightweight markup languages let you type a backslash (\) at the end of the line, but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. And at least a couple lightweight markup languages don’t require anything at the end of the line — just type return and they’ll create a line break.

✅  Do this	❌  Don't do this
First line with two spaces after.  
And the next line.

First line with the HTML tag after.<br>
And the next line.

First line with a backslash after.\
And the next line.

First line with nothing after.
And the next line.

Emphasis
You can add emphasis by making text bold or italic.

Bold
To bold text, add two asterisks or underscores before and after a word or phrase. To bold the middle of a word for emphasis, add two asterisks without spaces around the letters.

Markdown	HTML	Rendered Output
I just love **bold text**.	I just love <strong>bold text</strong>.	I just love bold text.
I just love __bold text__.	I just love <strong>bold text</strong>.	I just love bold text.
Love**is**bold	Love<strong>is</strong>bold	Loveisbold
Bold Best Practices
Markdown applications don’t agree on how to handle underscores in the middle of a word. For compatibility, use asterisks to bold the middle of a word for emphasis.

✅  Do this	❌  Don't do this
Love**is**bold	Love__is__bold
Italic
To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word for emphasis, add one asterisk without spaces around the letters.

Markdown	HTML	Rendered Output
Italicized text is the *cat's meow*.	Italicized text is the <em>cat's meow</em>.	Italicized text is the cat’s meow.
Italicized text is the _cat's meow_.	Italicized text is the <em>cat's meow</em>.	Italicized text is the cat’s meow.
A*cat*meow	A<em>cat</em>meow	Acatmeow
Italic Best Practices
Markdown applications don’t agree on how to handle underscores in the middle of a word. For compatibility, use asterisks to italicize the middle of a word for emphasis.

✅  Do this	❌  Don't do this
A*cat*meow	A_cat_meow
Bold and Italic
To emphasize text with bold and italics at the same time, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word for emphasis, add three asterisks without spaces around the letters.

Markdown	HTML	Rendered Output
This text is ***really important***.	This text is <em><strong>really important</strong></em>.	This text is really important.
This text is ___really important___.	This text is <em><strong>really important</strong></em>.	This text is really important.
This text is __*really important*__.	This text is <em><strong>really important</strong></em>.	This text is really important.
This text is **_really important_**.	This text is <em><strong>really important</strong></em>.	This text is really important.
This is really***very***important text.	This is really<em><strong>very</strong></em>important text.	This is reallyveryimportant text.
 Note: The order of the em and strong tags might be reversed depending on the Markdown processor you're using.
Bold and Italic Best Practices
Markdown applications don’t agree on how to handle underscores in the middle of a word. For compatibility, use asterisks to bold and italicize the middle of a word for emphasis.

✅  Do this	❌  Don't do this
This is really***very***important text.	This is really___very___important text.
Blockquotes
To create a blockquote, add a > in front of a paragraph.

> Dorothy followed her through many of the beautiful rooms in her castle.
The rendered output looks like this:

Dorothy followed her through many of the beautiful rooms in her castle.

Blockquotes with Multiple Paragraphs
Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
The rendered output looks like this:

Dorothy followed her through many of the beautiful rooms in her castle.

The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

Nested Blockquotes
Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
The rendered output looks like this:

Dorothy followed her through many of the beautiful rooms in her castle.

The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

Blockquotes with Other Elements
Blockquotes can contain other Markdown formatted elements. Not all elements can be used — you’ll need to experiment to see which ones work.

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
The rendered output looks like this:

The quarterly results look great!
Revenue was off the chart.
Profits were higher than ever.
Everything is going according to plan.

Blockquotes Best Practices
For compatibility, put blank lines before and after blockquotes.

✅  Do this	❌  Don't do this
Try to put a blank line before...

> This is a blockquote

...and after a blockquote.	Without blank lines, this might not look right.
> This is a blockquote
Don't do this!
Lists
You can organize items into ordered and unordered lists.

Ordered Lists
To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

Markdown	HTML	Rendered Output
1. First item
2. Second item
3. Third item
4. Fourth item	<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>	
First item
Second item
Third item
Fourth item
1. First item
1. Second item
1. Third item
1. Fourth item	<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>	
First item
Second item
Third item
Fourth item
1. First item
8. Second item
3. Third item
5. Fourth item	<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>	
First item
Second item
Third item
Fourth item
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item	<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ol>
      <li>Indented item</li>
      <li>Indented item</li>
    </ol>
  </li>
  <li>Fourth item</li>
</ol>	
First item
Second item
Third item
Indented item
Indented item
Fourth item
Ordered List Best Practices
CommonMark and a few other lightweight markup languages let you use a parenthesis ()) as a delimiter (e.g., 1) First item), but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. For compatibility, use periods only.

✅  Do this	❌  Don't do this
1. First item
2. Second item	1) First item
2) Second item
Unordered Lists
To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.

Markdown	HTML	Rendered Output
- First item
- Second item
- Third item
- Fourth item	<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>	
First item
Second item
Third item
Fourth item
* First item
* Second item
* Third item
* Fourth item	<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>	
First item
Second item
Third item
Fourth item
+ First item
+ Second item
+ Third item
+ Fourth item	<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>	
First item
Second item
Third item
Fourth item
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item	<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ul>	
First item
Second item
Third item
Indented item
Indented item
Fourth item
Starting Unordered List Items With Numbers
If you need to start an unordered list item with a number followed by a period, you can use a backslash (\) to escape the period.

Markdown	HTML	Rendered Output
- 1968\. A great year!
- I think 1969 was second best.	<ul>
  <li>1968. A great year!</li>
  <li>I think 1969 was second best.</li>
</ul>	
1968. A great year!
I think 1969 was second best.
Unordered List Best Practices
Markdown applications don’t agree on how to handle different delimiters in the same list. For compatibility, don’t mix and match delimiters in the same list — pick one and stick with it.

✅  Do this	❌  Don't do this
- First item
- Second item
- Third item
- Fourth item	+ First item
* Second item
- Third item
+ Fourth item
Adding Elements in Lists
To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

 Tip: If things don't appear the way you expect, double check that you've indented the elements in the list four spaces or one tab.
Paragraphs
* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.
The rendered output looks like this:

This is the first list item.
Here’s the second list item.

I need to add another paragraph below the second list item.

And here’s the third list item.
Blockquotes
* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list item.

* And here's the third list item.
The rendered output looks like this:

This is the first list item.
Here’s the second list item.

A blockquote would look great below the second list item.

And here’s the third list item.
Code Blocks
Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.
The rendered output looks like this:

Open the file.
Find the following code block on line 21:

 <html>
   <head>
     <title>Test</title>
   </head>
Update the title to match the name of your website.
Images
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.
The rendered output looks like this:

Open the file containing the Linux mascot.
Marvel at its beauty.

Tux, the Linux mascot

Close the file.
Lists
You can nest an unordered list in an ordered list, or vice versa.

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item
The rendered output looks like this:

First item
Second item
Third item
Indented item
Indented item
Fourth item
Code
To denote a word or phrase as code, enclose it in backticks (`).

Markdown	HTML	Rendered Output
At the command prompt, type `nano`.	At the command prompt, type <code>nano</code>.	At the command prompt, type nano.
Escaping Backticks
If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (``).

Markdown	HTML	Rendered Output
``Use `code` in your Markdown file.``	<code>Use `code` in your Markdown file.</code>	Use `code` in your Markdown file.
Code Blocks
To create code blocks, indent every line of the block by at least four spaces or one tab.

    <html>
      <head>
      </head>
    </html>
The rendered output looks like this:

<html>
  <head>
  </head>
</html>
 Note: To create code blocks without indenting lines, use fenced code blocks.
Horizontal Rules
To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

***

---

_________________
The rendered output of all three looks identical:

Horizontal Rule Best Practices
For compatibility, put blank lines before and after horizontal rules.

✅  Do this	❌  Don't do this
Try to put a blank line before...

---

...and after a horizontal rule.	Without blank lines, this would be a heading.
---
Don't do this!
Links
To create a link, enclose the link text in brackets (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., (https://duckduckgo.com)).

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
The rendered output looks like this:

