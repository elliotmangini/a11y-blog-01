# a11y-blog-01

<h1>A11y Accessibility</h1>

<h2><em><a href="https://www.a11yproject.com/">The A11y Project</a> ("A"-eleven-"Y") is a community driven effort to make digital accessibility easier.</em><h2>

<h3>Accessibility is the goal of incorporating a set of practices and principles that make your application, website, or product useful for a broader audience. It is in nature a humanitarian effort, and the following is my small contribution to the above community effort, which aims to help newer developers establish a big picture overview of what it means to
incorporate great accessibility practices.</h3>

<p>
While completing a Full Stack bootcamp in 2022 I learned a ton about web development, but one of the things that gets overlooked in programs like the one I did is accessibility.
This is common in these types of programs because the focus is on building projects and gaining practical experience, which is a great fit for the stage of learning most bootcamp attendees are at. If you have recently finished a bootcamp and are considering what to learn next, accessibility is a great way to make yourself more valuable as an engineer, expand your understanding of technology and improve your decision-making in your day-to-day workflow. Accessibility best practices are often about providing options but they're also about organizing information in a way that will make it useful to the largest number of people. The best way to create stellar accessibility
in your projects is to think about it from the start as you work on a project. If you wait until the end of your project, making it accessible can be expensive and time-consuming. So
as an engineer, one of the most valuable things you can offer is to be someone who writes beautiful, clean, accessible code from the start. An important thing to understand is that
when done correctly, the investment in creating a robust inclusive experience pays off.
</p>

<h2>Who benefits from accessibility?</h2>
<ul>
<li>Physical Limitations: <em>Using a mouse, using a keyboard, using a touchscreen, using your voice.</em></li>

<li>Cognitive Disabilities: <em>ADHD, Dislexia, Autism, Down Syndrome, Traumatic Brain Injury, Seizure Disorders (this is the largest and most varied group!)</em></li>

<li>Visual Disabilities: <em>Blindness, Color Blindness</em></li>

<li>Audio: <em>Deafness, Captioning, Sign Language Interpretation, Video with Audio, Hardness of hearing.</em></li>
</ul>

<strong>Accessibility benefits everyone.</strong>

<em>Accessibility is not just about ensuring that your text is visible on a black background, but rather considering the needs of a diverse range of individuals.</em>


<h2>Where do we learn about accessibility best practices?</h2>

IMAGE CARIE FISHER

<p>This blog serves as a brief guide and overview of the topics covered in <a href="https://www.youtube.com/live/oEiTjDMA7UU?feature=share">Carie Fisher's Web Accessibility 101 Seminar</a>, which is a one hour live stream provided by Fisher, a Senior Accessibility Trainer.</p>

<h1>Terminology</h1>

<strong>AT devices/AT Compatible</strong>
<br>
<p>
    Assistive Technology (Devices) can refer to screen readers, keyboards, displays that magnify, but also things like Google Assistant/Siri. Any technologies that allow someone to organize what their viewing in a way that works for them.
</p>

<strong>Accessibility Overlays</strong>
<br>
<p>
    Accessibility Overlays are technologies and strategies that we can slap onto legacy code to improve its accessibility either as
    developers or in some cases as users.
</p>

<h1>Developing an Accessibility Plan</h1>

<p>
    We will adopt a good, better, best approach. Fisher explains in the seminar that when we wait until the end to implement accsibility we tend to start at the bottom of our "pyramid" of needs, which imagines those at the top as a group dependent on the narrowest window of informational presentation
    formats, and those at the bottom as being limited in some ways but able to utilize a wider range of designs than those at
    the top. However, when we begin by presenting our information in a way that works for folks at the top, it generally has the effect of
    making our product work for everyone below them on the pyramid too. "Good" might be implementing good contrast practices, "Better" might be using a many-pronged approach where we're also offering choices between different fonts too-- and "Best" might be where we are doing those things, but where our primary concern and starting point is making sure our information is presented in an order that makes it easy to follow, where we're offering images for visual learners and text for folks who absorb information best by reading, and videos for folks who learn best that way-- where we're optimized for screen readers, for use without a mouse, across different screens etc. etc. and thinking about our designs in terms of the whole being greater than the sum of the parts.
</p>

<p>
    According to Fisher, the most important tenant of accessibility is the skeleton. And I really love this approach, because it tickles
    the part of my brain that thinks about visual design (an area where I have more experience) as being much more than aesthetics. The idea that where we put information and how "big" it is, or even <em>when we encounter it</em> is the <em>biggest</em>
    thing that determines how readily we can follow along and relate to what we're engaging with. AT tools typically address the top level, such as ensuring the focus highlighting is large and visible or giving users control over font size, but we want to adopt a mindset where we understand that...
</p>

<em>Tools that only address the top level cannot fix poor design language.</em>


<h3>Familiarizing ourselves with accessibility strategies</h3>
<ul>
    <li>Informational Heirarchy</li>
    <li>Screen Readers</li>
    <li>Contrast</li>
    <li>Fonts</li>
    <li>Device Accomodations</li>
</ul>

<h2>Informational Heirarchy & Design Language</h2>

<p>We will first discuss the main goal, the skeleton, structure, and HTML, and then move on to tips that focus on the middle of the pyramid. When using a screen reader, the HTML is the biggest factor in determining the accessibility of the content. So how do we write legible HTML?</p>

<h3>Great HTML</h3>

<ul>
<li>Use semantic HTML: Use the appropriate HTML element for the type of content it contains, such as lists for lists, quotes for quotes, p for paragraphs etc. This provides information about the structure and purpose of the content to assistive technology.</li>

<li>Use heading structure: Use the HTML heading tags (H1-H6) to structure the content of the page, with H1 being the main heading and H2-H6 being subheadings. This helps users understand the page structure and allows assistive technology to accurately navigate the page.</li>

<li>Use descriptive link text: Use descriptive link text that clearly describes the purpose or destination of the link. Avoid using generic text such as "click here".</li>

<li>Use tables appropriately: Use tables only for tabular data, not for layout purposes. Use the appropriate table elements such as TH for header cells and TD for data cells to provide context and structure to the table.</li>

<li>Organize content with ordered and unordered lists: Use ordered and unordered lists to organize content into manageable sections, making it easier to read and understand.</li>

<li>Use descriptive title and alt attributes: Use the title and alt attributes to provide descriptive text for images, links, and other elements. This provides additional information to assistive technology and is also used to display a text description for images that do not load properly.</li>

<li>Use ARIA attributes: Use ARIA (Accessible Rich Internet Applications) attributes to provide additional information about the purpose and role of elements on the page, such as a landmark region, a tooltip, or a dialog box.</li>
</ul>

<p>
    It may sound overly simplified, but after working with a senior developer friend and improving my skills, I have come to realize that using code (especially HTML tags) for their intended purpose (as outlined in item 1) is key.
</p>

<h3>Quick Tips</h3>

<p>
The following tips are based on the Web Content Accessibility Guidelines (WCAG) and Fisher's personal perspective on accessibility.

<strong>Provide text alternatives for non-text content:</strong> All non-text content such as images, videos, and audio files should have text descriptions or transcripts that can be read by assistive technology.

<strong>Use sufficient contrast:</strong> The contrast between text and its background must be high enough to ensure readability for people with visual impairments. To get more granular, The color contrast ratio between text and its background must be at least 4.5:1 for regular text and 3:1 for large text (24 point or larger and bold text or 19 point or larger).

You can use online tools such as the <a href="https://webaim.org/resources/contrastchecker/">WebAIM Color Contrast Checker</a> or the Accessibility Checker in Adobe Photoshop to test your color contrast and see if it meets the minimum requirements. It's important to keep in mind that while this is a general rule, there may be exceptions for logos, graphs, and charts, among other things. It's always best to consult the WCAG guidelines directly for a more complete understanding of the requirements.

Fisher suggests using the <a href="https://www.tpgi.com/color-contrast-checker/">Color Contrast Analyzer</a> by TPGi for checking contrast because it can analyze the code itself. But let's breifly look at how to perform a manual check to find problems that the automated checker can't catch.

We can select colors on our page using this checker by selecting the background color first...
</p>

IMAGE

<p>Then, selecting the font color...</p>

IMAGE

<p>Now we can see our contrast ratio-- in this case, 1.57:1, which according to Fisher is "horrible".</p>

IMAGE

<p>
    In her demonstration, Fisher goes on to resize the window and check the same area on screen. This demonstrates how the contrast ratios a user encounters can change as the elements move around.
</p>

IMAGE

<p>These kinds of checkers can highlight problems of many kinds, for example showing us whether elements are focusable when we might want them to be. Fisher says by far this is her favorite one!</p>

<ul>
<li><strong>Provide visual cues for audio content:</strong> For audio content such as videos or podcasts, provide visual cues such as captions or transcripts to make it accessible to people with hearing impairments.</li>

<li><strong>Avoid flashing content:</strong> Avoid using flashing or blinking content, as it can cause seizures in people with photosensitive epilepsy.</li>

<li><strong>Make sure content is resizeable:</strong> Web content must be scalable and readable without the need for zooming, as many people with visual impairments may not be able to use a mouse or trackpad to zoom in on the content.</li>

<li><strong>Provide context for icons:</strong> When using icons, ensure that they are accompanied by text that provides context or a clear label that explains their meaning. This will make the content more accessible to users with visual impairments or cognitive disabilities who may have difficulty understanding the purpose of an icon on its own.</li>
</ul>

<h2>Fonts</h2>

IMAGE DYSLEXIE, COMIC SANS, & ATKINSON EXAMPLES

<p>Fonts where each character is very distinct. To my surprise, comic sans is a very accessible font. But when you know what makes a font accessible it makes sense! Dyslexie and Atkinson Hyperlegible are two fonts that are designed specifically to be useful for individuals with dislexia.</p>

IMAGE ARIAL
<p>
    However, Arial is a font that individuals with dyslexia have encountered many times. Studies have found that Arial is just as good as these specialty fonts in terms of reading comprehension and speed.
    So it isn't always intuitive which choices will work for a largest number of users.
</p>

IMAGE CURSIVE & INDISTINCT CHARACTER EXAMPLES

<p>
    Font choice largely comes down to personal preference. But avoiding cursive fonts, since cursive is no longer taught in schools, or
    avoiding fonts that do not have distinct characters can be a great place to start.
</p>

<h2>Providing Options</h2>
<p>Now with the above in mind, you can do something like implementing a toggles for different fonts, but you can also do something like not locking down your CSS so that someone can utilize their own style sheets using an AT tool or Screen Reader or something that would allow them to control how the page looks.</p>

<h1>Conclusions</h1>

<p>Accessibility is a crucial aspect of web development that is often overlooked due to the fast pace of most bootcamp programs. However, it is an important area for new developers to focus on as it helps make applications, websites, and products useful for a wider audience, including those with physical, cognitive, and visual disabilities. Developing with great accessibility doesn't take extra time <em>most
of the time</em>, it just requires an awareness of a few basic principles, and that awareness can actually help us make decisions more easily about where to put what and how to do things. Hopefully, this brief introduction to key terms and concepts, and overview of how to develop and incorporate an accessibility plan will help you as you encounter new codebases and begin to make more specific decisions with
regard to accessibility. By making accessibility a priority, we can create a more inclusive and accessible digital world for all.</p>