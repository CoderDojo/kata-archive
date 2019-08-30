You can format your text by using wiki markup. This consists of normal
characters like asterisks, apostrophes or equal signs which have a
special function in the wiki, sometimes depending on their position. For
example, to format a word in *italic*, you include it in two pairs of
apostrophes like `''this''`.

## Text formatting markup

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 40%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Description</p></th>
<th><p>You type</p></th>
<th><p>You get</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Character (inline) formatting – <em>applies anywhere</em></p></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><p>Italic text</p></td>
<td><pre><code>&#39;&#39;italic&#39;&#39;</code></pre></td>
<td><p><em>italic</em></p></td>
</tr>
<tr class="odd">
<td><p>Bold text</p></td>
<td><pre><code>&#39;&#39;&#39;bold&#39;&#39;&#39;</code></pre></td>
<td><p><strong>bold</strong></p></td>
</tr>
<tr class="even">
<td><p>Bold and italic</p></td>
<td><pre><code>&#39;&#39;&#39;&#39;&#39;bold &amp; italic&#39;&#39;&#39;&#39;&#39;</code></pre></td>
<td><p><strong><em>bold &amp; italic</em></strong></p></td>
</tr>
<tr class="odd">
<td><p>Strike text</p></td>
<td><pre><code>&lt;strike&gt;strike text&lt;/strike&gt;</code></pre></td>
<td><p><del>strike text</del></p></td>
</tr>
<tr class="even">
<td><p>Escape wiki markup</p></td>
<td><pre><code>&amp;lt;nowiki&amp;gt;no &#39;&#39;markup&#39;&#39;&amp;lt;/nowiki&amp;gt;</code></pre></td>
<td><p>no ''markup''</p></td>
</tr>
<tr class="odd">
<td><p>Escape wiki markup once</p></td>
<td><pre><code>[[Special:MyLanguage/API:Main page|API]]&amp;lt;nowiki/&gt;&amp;nbsp;
extension</code></pre></td>
<td><p><a href="Special:MyLanguage/API:Main_page" title="wikilink">API</a>  extension</p></td>
</tr>
<tr class="even">
<td><p>Section formatting – <em>only at the beginning of the line</em></p></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><p>Headings of different levels</p></td>
<td><pre><code>
== Level 2 == 

=== Level 3 === 

==== Level 4 ==== 

===== Level 5 ===== 

====== Level 6 ====== </code></pre></td>
<td><h2>
<p>Level 2</p>
</h2>
<h3>
<p>Level 3</p>
</h3>
<h4>
<p>Level 4</p>
</h4>
<h5>
<p>Level 5</p>
</h5>
<h6>
<p>Level 6</p>
</h6></td>
</tr>
<tr class="even">
<td><p>Horizontal rule</p></td>
<td><pre><code>
Text before
----

Text after</code></pre></td>
<td><p>Text before</p>
<hr />
<p>Text after</p></td>
</tr>
<tr class="odd">
<td><p>Bullet list</p></td>
<td><pre><code>

* Start each line
* with an [[Wikipedia:asterisk|asterisk]] (*).
** More asterisks give deeper
*** and deeper levels.
* Line breaks &lt;br /&gt;don&#39;t break levels.
*** But jumping levels creates empty space.
Any other start ends the list.</code></pre></td>
<td><ul>
<li>Start each line</li>
<li>with an <a href="Wikipedia:asterisk" title="wikilink">asterisk</a> (*).
<ul>
<li>More asterisks give deeper
<ul>
<li>and deeper levels.</li>
</ul></li>
</ul></li>
<li>Line breaks<br />
don't break levels.
<ul>
<li><ul>
<li>But jumping levels creates empty space.</li>
</ul></li>
</ul></li>
</ul>
<p>Any other start ends the list.</p></td>
</tr>
<tr class="even">
<td><p>Numbered list</p></td>
<td><pre><code>

# Start each line
# with a [[Wikipedia:Number_sign|number sign]] (#).
## More number signs give deeper
### and deeper
### levels.
# Line breaks &lt;br /&gt;don&#39;t break levels.
### But jumping levels creates empty space.
# Blank lines


# end the list and start another.
Any other start also
ends the list.</code></pre></td>
<td><ol>
<li>Start each line</li>
<li>with a <a href="Wikipedia:Number_sign" title="wikilink">number sign</a> (#).
<ol>
<li>More number signs give deeper
<ol>
<li>and deeper</li>
<li>levels.</li>
</ol></li>
</ol></li>
<li>Line breaks<br />
don't break levels.
<ol>
<li><ol>
<li>But jumping levels creates empty space.</li>
</ol></li>
</ol></li>
<li>Blank lines</li>
</ol>
<ol>
<li>end the list and start another.</li>
</ol>
<p>Any other start also ends the list.</p></td>
</tr>
<tr class="odd">
<td><p>Definition list</p></td>
<td><pre><code>

;item 1
: definition 1
;item 2
: definition 2-1
: definition 2-2</code></pre></td>
<td><dl>
<dt>item 1</dt>
<dd>definition 1
</dd>
<dt>item 2</dt>
<dd>definition 2-1
</dd>
<dd>definition 2-2
</dd>
</dl></td>
</tr>
<tr class="even">
<td><p>Indent text</p></td>
<td><pre><code>

: Single indent
:: Double indent
::::: Multiple indent</code></pre>
<hr />
<p><em>Note:</em> This workaround may harm accessibility.</p></td>
<td><dl>
<dt></dt>
<dd>Single indent
<dl>
<dt></dt>
<dd>Double indent
<dl>
<dt></dt>
<dd><dl>
<dt></dt>
<dd>Multiple indent
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl></td>
</tr>
<tr class="odd">
<td><p>Mixture of different types of list</p></td>
<td><pre><code>

# one
# two
#* two point one
#* two point two
# three
#; three item one
#: three def one
# four
#: four def one
#: this looks like a continuation
#: and is often used
#: instead &lt;br /&gt;of &amp;lt;nowiki&gt;&lt;br /&gt;&amp;lt;/nowiki&gt;
# five
## five sub 1
### five sub 1 sub 1
## five sub 2</code></pre>
<hr />
<p><em>Note:</em> The usage of <code>#:</code> and <code>*:</code> for breaking a line within an item may also harm accessibility.</p></td>
<td><ol>
<li>one</li>
<li>two
<ul>
<li>two point one</li>
<li>two point two</li>
</ul></li>
<li>three
<dl>
<dt>three item one</dt>
<dd>three def one
</dd>
</dl></li>
<li>four
<dl>
<dt></dt>
<dd>four def one
</dd>
<dd>this looks like a continuation
</dd>
<dd>and is often used
</dd>
<dd>instead<br />
of &lt;br /&gt;
</dd>
</dl></li>
<li>five
<ol>
<li>five sub 1
<ol>
<li>five sub 1 sub 1</li>
</ol></li>
<li>five sub</li>
</ol></li>
</ol></td>
</tr>
<tr class="even">
<td><p>Preformatted text</p></td>
<td><pre><code>
 
Start each line with a space.
 Text is &#39;&#39;&#39;preformatted&#39;&#39;&#39; and
 &#39;&#39;markups&#39;&#39; &#39;&#39;&#39;&#39;&#39;can&#39;&#39;&#39;&#39;&#39; be done.</code></pre>
<hr />
<p>Note:'' This way of preformatting only applies to section formatting. Character formatting markups are still effective.</p></td>
<td><p>Start each line with a space.</p>
<p><code>Text is </code><strong><code>preformatted</code></strong><code> and</code><br />
<em><code>markups</code></em><code> </code><strong><em><code>can</code></em></strong><code> be done.</code></p></td>
</tr>
</tbody>
</table>

## Paragraphs

MediaWiki ignores single line breaks. To start a new paragraph, leave an
empty line. You can force a line break within a paragraph with the HTML
tag `<br />`.

## HTML tags

Some HTML tags are allowed in MediaWiki, for example `<code>`, `<div>`,
`<span>` and `<font>`. These apply anywhere you insert them.

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 40%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Description</p></th>
<th><p>You type</p></th>
<th><p>You get</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Inserted<br />
(Displays as underline in most browsers)</p></td>
<td><pre><code>&lt;ins&gt;Inserted&lt;/ins&gt;


or

&lt;u&gt;Underline&lt;/u&gt;</code></pre></td>
<td><p><ins>Inserted</ins></p>
<p>or</p>
<p><u>Underline</u></p></td>
</tr>
<tr class="even">
<td><p>Deleted<br />
(Displays as strikethrough in most browsers)</p></td>
<td><pre><code>&lt;s&gt;Struck out&lt;/s&gt;


or

&lt;del&gt;Deleted&lt;/del&gt;</code></pre></td>
<td><p><s>Struck out</s></p>
<p>or</p>
<p><del>Deleted</del></p></td>
</tr>
<tr class="odd">
<td><p>Fixed width text</p></td>
<td><pre><code>&lt;code&gt;Source code&lt;/code&gt;


or

&lt;tt&gt;Fixed width text&lt;/tt&gt;</code></pre></td>
<td><p><code>Source code</code></p>
<p>or</p>
<p><code>Fixed width text</code></p></td>
</tr>
<tr class="even">
<td><p>Blockquotes</p></td>
<td><pre><code>
Text before
&lt;blockquote&gt;Blockquote&lt;/blockquote&gt;

Text after</code></pre></td>
<td><p>Text before</p>
<blockquote>
<p>Blockquote</p>
</blockquote>
<p>Text after</p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><pre><code>
&lt;!-- This is a comment --&gt;
Comments are visible only 
in the edit zone.</code></pre></td>
<td><p>Comments are visible only in the edit zone.</p></td>
</tr>
<tr class="even">
<td><p>Completely preformatted text</p></td>
<td><pre><code>&lt;pre&gt;

Text is &#39;&#39;&#39;preformatted&#39;&#39;&#39; and 
&#39;&#39;markups&#39;&#39; &#39;&#39;&#39;&#39;&#39;cannot&#39;&#39;&#39;&#39;&#39; be done&amp;lt;/pre&gt;</code></pre>
<hr />
<p>Note: For marking up of preformatted text, check the &quot;Preformatted text&quot; entry at the end of the previous table.</p></td>
<td><pre><code>
Text is &#39;&#39;&#39;preformatted&#39;&#39;&#39; and 
&#39;&#39;markups&#39;&#39; &#39;&#39;&#39;&#39;&#39;cannot&#39;&#39;&#39;&#39;&#39; be done</code></pre></td>
</tr>
<tr class="odd">
<td><p><strong>Customized</strong> preformatted text</p></td>
<td><pre><code>&lt;pre style=&quot;color: red&quot;&gt;

Text is &#39;&#39;&#39;preformatted&#39;&#39;&#39; 
with a style and 
&#39;&#39;markups&#39;&#39; &#39;&#39;&#39;&#39;&#39;cannot&#39;&#39;&#39;&#39;&#39; be done
&amp;lt;/pre&gt;</code></pre>
<hr />
<p>Note: A CSS style can be named within the <code>style</code> property.</p></td>
<td><pre><code>
Text is &#39;&#39;&#39;preformatted&#39;&#39;&#39; 
with a style and 
&#39;&#39;markups&#39;&#39; &#39;&#39;&#39;&#39;&#39;cannot&#39;&#39;&#39;&#39;&#39; be done</code></pre></td>
</tr>
</tbody>
</table>

continued:

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 40%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Description</p></th>
<th><p>You type</p></th>
<th><p>You get</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Customized</strong> preformatted text with text wrap according to available width</p></td>
<td><pre><code>&lt;pre style=&quot;white-space: pre-wrap; 
white-space: -moz-pre-wrap; 
white-space: -pre-wrap; 
white-space: -o-pre-wrap; 
word-wrap: break-word;&quot;&gt;

This long sentence is used to demonstrate text wrapping. This additional sentence makes the text even longer.
&amp;lt;/pre&gt;</code></pre></td>
<td><pre><code>
This long sentence is used to demonstrate text wrapping. This additional sentence makes the text even longer.</code></pre></td>
</tr>
<tr class="even">
<td><p>Preformatted text with text wrap according to available width</p></td>
<td><pre><code>&lt;code&gt;

This long sentence is used to demonstrate text wrapping. This additional sentence makes the text even longer.
&lt;/code&gt;</code></pre></td>
<td><p><code></p>
<p>This long sentence is used to demonstrate text wrapping. This additional sentence makes the text even longer. </code></p></td>
</tr>
</tbody>
</table>

## Inserting symbols

Symbols and other special characters not available on your keyboard can
be inserted through a special sequence of characters. Those sequences
are called HTML entities. For example, the following sequence (entity)
**\&rarr;** when inserted will be shown as <ins>right arrow</ins> HTML
symbol → and **\&mdash;** when inserted will be shown as an <ins>em
dash</ins> HTML symbol —.

-----

Note: Hover over any character to find out the symbol that it produces.
Some symbols not available in the current font will appear as empty
squares.

| HTML symbol entities                   |
| -------------------------------------- |
| '''<span title="&amp;Aacute;">Á</span> |
| '''<span title="&amp;Chi;">Χ</span>    |
| '''<span title="&amp;ETH;">Ð</span>    |
| '''<span title="&amp;iquest;">¿</span> |
| '''<span title="&amp;ne;">≠</span>     |
| '''<span title="&amp;ouml;">ö</span>   |
| '''<span title="&amp;rsaquo;">›</span> |
| '''<span title="&amp;times;">×</span>  |

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 40%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Description</p></th>
<th><p>You type</p></th>
<th><p>You get</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Copyright symbol</p></td>
<td><p><tt></p>
<pre><code>&amp;amp;copy;</code></pre>
<p></tt></p></td>
<td><dl>
<dt></dt>
<dd><dl>
<dt></dt>
<dd><strong>©</strong>
</dd>
</dl>
</dd>
</dl></td>
</tr>
<tr class="even">
<td><p>Greek delta letter symbol</p></td>
<td><p><tt></p>
<pre><code>&amp;amp;delta;</code></pre>
<p></tt></p></td>
<td><dl>
<dt></dt>
<dd><dl>
<dt></dt>
<dd><strong>δ</strong>
</dd>
</dl>
</dd>
</dl></td>
</tr>
<tr class="odd">
<td><p>Euro currency symbol</p></td>
<td><p><tt></p>
<pre><code>&amp;amp;euro;</code></pre>
<p></tt></p></td>
<td><dl>
<dt></dt>
<dd><dl>
<dt></dt>
<dd><strong>€</strong>
</dd>
</dl>
</dd>
</dl></td>
</tr>
</tbody>
</table>

See the list of all HTML entities on the Wikipedia article [List of HTML
entities](wikipedia:List_of_HTML_entities.md). Additionally,
MediaWiki supports two non-standard entity reference sequences: `&רלמ;`
and `&رلم;` which are both considered equivalent to `&rlm;` which is a
[right-to-left mark](wikipedia:Right-to-left_mark.md). (Used
when combining right to left languages with left to right languages in
the same
page.)

## HTML tags and symbol entities displayed themselves (with and without interpreting them)

  -   
    `&amp;euro;`  → **\&euro;**

<!-- end list -->

  -   
    <tt>\<span style="color: red; text-decoration: line-through;"\>

Typo to be corrected\</span\></tt>  →
**<span style="color: red; text-decoration: line-through;"> Typo to be
corrected</span>**

  -   
    <tt>

\&lt;span style="color: red; text-decoration: line-through;"\>Typo to be
corrected\</span\></tt>  → **\<span style="color: red; text-decoration:
line-through;"\> Typo to be corrected\</span\>**

### Nowiki for HTML

\<nowiki /\> can prohibit (HTML) tags:

  - \<\<nowiki /\>pre\>  → \<pre\>

But *not* & symbol escapes:

  - &\<nowiki /\>amp;  → &

To print & symbol escapes as text, use "`&amp;`" to replace the "&"
character (eg. type "`&amp;nbsp;`", which results in "`&nbsp;`").
