Download Link: https://assignmentchef.com/product/solved-cinf201-week4-html-ii
<br>
<h1>Overview</h1>

This week we will learn about semantic tags in HTML. These are tags which help define our content more appropriately and can be helpful for usability/accessibility. We will also cover validating our HTML and how to make our web pages live so that other people can visit them.

Project Proposal

The first part of the final project (Project Proposal) is due on September 30<sup>th</sup> at midnight. You will need to submit 3 wireframes, 1 style tile, and 1 needs assessment for the website you plan to build for your final project. If you aren’t sure about your topic or the quality of your proposal, please reach out to me.




<strong>Previous Participation Questions/Responses </strong>These are the participation questions from last week:

<u>https://forms.gle/4DQPbvaF4r6hP1y77</u>




This link has the responses to the fun question from last week. Feel free to look over the responses from myself and your peers.  <u>https://docs.google.com/spreadsheets/d/1QLoQzbO-</u>

<u>Er7ARIECl0aPvY1lKUyZTdYeuwsn4g0XEAk/edit?usp=sharing</u>




<h1>More HTML Fun (Lecture/Class Activity)</h1>

<h2>HTML Review</h2>

Last week, we learned about HTML and discussed the various components which make up an HTML element. Below is an example that was included in last week’s lecture notes. There are 4 total parts to an HTML element:




<h2>&lt;p class=“para”&gt;This is a paragraph.&lt;/p&gt;</h2>




&lt;p&gt; and &lt;/p&gt; are the <u>opening and closing tags</u>.




class is an <u>attribute</u>.




“para” is the <u>value</u> provided for the attribute.




“This is a paragraph.” is the <u>content</u> between the tags.




Tags, attributes, values, and content can all be used to build an HTML element. At the very least, you will need to utilize tags/content to get items displaying on your page.




Feel free to follow along with me as I do a brief demonstration of the tags again to recap some of what was covered last week. Afterward, I will introduce new HTML tags (semantic tags).

<strong> </strong>

<h2>Semantic Tags in HTML</h2>

For web pages, the browser interprets the tags used in the .html file and displays them as it comes across them. We can do things like create headings, paragraphs, images, etc. using specific tags intended for those purposes. If we choose to use tags for purposes they weren’t intended for, it could have consequences for users. Of course, we can use things like CSS/JS to cover up poor HTML structure but that only works for entirely visual users.




One example of improper tag usage is when a developer uses table-related tags to create a layout for a page. Div, section, main, aside, and other semantic tags are better suited for the purposes of creating a layout. Screen readers most likely will not read the content in the order you intended if you use a table for layouts.




If we want our page to be as accessible/usable for as many users as possible, it is important to use semantic markup correctly. Any tags we use should help define the document structure in a clear manner and separate content from styles. This will allow users that utilize tools like screen readers to access our content and create a better experience overall.




A lot of web developers tend to use div tags to markup their content as they are useful as containers. However, divs aren’t very useful for non-visual users as they don’t offer any information as to the nature of the content inside of them. It can be difficult to build a complete page without using divs, but you should do your best to use semantic markup when possible.













Examples of common semantic tags:




<table width="623">

 <tbody>

  <tr>

   <td width="126"><strong>Tag Names </strong></td>

   <td width="498"><strong>Purpose </strong></td>

  </tr>

  <tr>

   <td width="126">Header</td>

   <td width="498">Represents introductory content such as navigation menus</td>

  </tr>

  <tr>

   <td width="126">Nav</td>

   <td width="498">Contains navigation-based links in major blocks</td>

  </tr>

  <tr>

   <td width="126">Aside</td>

   <td width="498">Usually used for content aside from the main content such as sidebars</td>

  </tr>

  <tr>

   <td width="126">Main</td>

   <td width="498">Contains the main content for a document</td>

  </tr>

  <tr>

   <td width="126">Article</td>

   <td width="498">Independent content such as forum or blog posts</td>

  </tr>

  <tr>

   <td width="126">Section</td>

   <td width="498">This identifies sections in a document and is sometimes used in article tags</td>

  </tr>

  <tr>

   <td width="126">Footer</td>

   <td width="498">Defines a footer for a document or section</td>

  </tr>

 </tbody>

</table>




<u>Additional Reading</u>

<ul>

 <li><u>https://html.com/semantic-markup/</u></li>

 <li><u>https://www.lifewire.com/why-use-semantic-html-3468271</u></li>

 <li><u>https://internetingishard.com/html-and-css/semantic-html/</u></li>

</ul>




<h2>HTML Validation</h2>

For our pages to present themselves correctly and behave in expected ways, it is important to validate our documents. A document’s code is considered valid when the tags are nested correctly, and everything is placed according to W3C specifications. An example would be a &lt;ul&gt; tag containing only &lt;li&gt; elements inside of it. One rule that trips up students a lot is that &lt;ul&gt; cannot be a direct child of another &lt;ul&gt; (same for &lt;ol&gt;). The sample code below demonstrates good and bad structures for lists.







<table width="623">

 <tbody>

  <tr>

   <td width="312"><strong>Good List Structure </strong></td>

   <td width="312"><strong>Bad List Structure </strong></td>

  </tr>

  <tr>

   <td width="312">&lt;ul&gt;&lt;li&gt;Item 1&lt;/li&gt;&lt;li&gt;Item 2&lt;ul&gt;&lt;li&gt;Sub Item 1&lt;/li&gt;&lt;/ul&gt;&lt;/li&gt;&lt;li&gt;Item 3&lt;/li&gt;&lt;/ul&gt; </td>

   <td width="312">&lt;ul&gt;&lt;li&gt;Item 1&lt;/li&gt;&lt;li&gt;Item 2&lt;/li&gt;&lt;ul&gt;&lt;li&gt;Sub Item 1&lt;/li&gt; &lt;/ul&gt;&lt;li&gt;Item 3&lt;/li&gt;&lt;/ul&gt; </td>

  </tr>

 </tbody>

</table>




In the example above, the left side has the 2<sup>nd</sup> &lt;ul&gt; tag nested <strong>inside</strong> of the 2<sup>nd</sup> &lt;li&gt; tag. The &lt;/li&gt; tag is closed <strong>after</strong> the 2<sup>nd</sup> &lt;ul&gt; set is closed. In the bad list portion, the 2<sup>nd</sup> &lt;ul&gt; is a direct child of the 1<sup>st</sup> &lt;ul&gt; and therefore not valid. This is just a rule that is a standard in HTML and there are many others like it.




I don’t expect you all to memorize all rules; you can use a validator instead. It will tell you what lines of code are wrong, so you can fix them and improve your document’s markup. To check your code, copy all of it and paste it directly into the validator. You can also upload files or provide a link but copy/pasting code is quicker.




Use the website below to validate your code in the assignment mentioned below. I would recommend bookmarking it in your favorite browser for the semester. Chrome is my browser of choice, but Edge and Firefox are pretty good as well. A green bar means your document validates perfectly.




<u>https://validator.w3.org/#validate_by_input</u>




<h2>Publishing Our Web Pages</h2>

To publish our web pages, we need to use FTP software to place our files on the UAlbany server. Each of you has space reserved for hosting files and we will use that space for our coursework this semester.




Follow along with me as I demonstrate how to upload files using FileZilla. If you get lost or I’m going too fast, feel free to refer to the “Viewing our Web Pages.docx” document that has been provided with today’s lecture notes. If you ever forget how to do the file upload, this document is also available on Blackboard through Course Materials à Additional Resources.




<h1>Validation Exercise (CW)</h1>

Download the validation-exercise.zip folder from Blackboard under today’s lecture notes or the assignments folder. After you have downloaded the folder, extract the files to somewhere else on your computer where you’ll be able to find them.

Your task is to fix the HTML in the document which contains numerous errors. To see what your page should look like after you have fixed it, there is an image included in the zip folder.

The content on the page goes beyond the height of the screen so the image provided will look small as I took a scrolling screenshot of it. However, you can zoom in on the image and everything should be clear to see. If you experience issues with image visibility, please contact me.

<strong>No text content inside of tags should be added/removed from the page</strong>, but you will need to add, delete, alter, or move around tags.

To validate your page, visit the following link and enter your code:  <u>https://validator.w3.org/#validate_by_input</u>

Once your page is validated, place it on your UAlbany server area as explained earlier in class today. To earn credit for this assignment, you will need to submit a link to a validated page to Blackboard. You will know the page is validated when you use the validator link and it displays a green bar with the text: <strong>Document checking completed. No errors or warnings to show.  </strong>

<u>Tips</u>