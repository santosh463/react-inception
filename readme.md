Episode 1- Inception

<ul>
    What is Emmet?
    <li>“Emmet is a plug in for many popular text editors which greatly improves HTML & CSS workflow:”
        And Emmet does fulfill what they promise, you can use short expressions to generate HTML markup, CSS.</li>
</ul>

<ul>

    The technical difference between a framework and a library is defined by a concept known as inversion of
    control. When you use a library, you control the application flow, including when and where to contact the
    library. When you use a framework, the framework itself controls the flow. There are some other distinctions
    between libraries and frameworks as well. Let’s have a look at a couple of the most important ones:
    <div style="display: flex;justify-content: space-around;">
        <div>
            <div>
                Library
                <li>A set of assistance modules, objects, classes, functions, pre-written code, and so on.</li>
                <li>Can be easily substituted by another library.</li>
                <li>When we call a method from a library, we are in control.</li>
                <li>Since developing a library needs less code, performance and load time are improved.</li>
                <li> Libraries can be simply linked into existing programs to add specific functionality. </li>
            </div>
        </div>
        <div>
            <div>Framework

                <li>Includes a variety of APIs, compilers, support applications, libraries, and so on.</li>
                <li>Are tough to replace.</li>
                <li>Inversion of control, i.e. the framework calls us.</li>
                <li>The construction of a
                    framework necessitates large amounts of code, which reduces performance and increases load time.
                </li>
                <li>It is tough to incorporate
                    a framework seamlessly into an existing project.</li>
            </div>
        </div>
    </div>
</ul>

<ul>
    What is a CDN?
    <li>A content delivery network (CDN) is a network of interconnected servers that speeds up webpage loading for
        data-heavy applications. CDN can stand for content delivery network or content distribution network. When a user
        visits a website, data from that website's server has to travel across the internet to reach the user's
        computer. If the user is located far from that server, it will take a long time to load a large file, such as a
        video or website image. Instead, the website content is stored on CDN servers geographically closer to the users
        and reaches their computers much faster.</li>
</ul>

<ul>What is crossorigin in script tag
    <li>The purpose of crossorigin attribute is used to share the resources from one domain to another domain.
        Basically, it is used to handle the CORS request. It is used to handle the CORS request that checks whether it
        is safe to allow for sharing the resources from other domains.</li>
</ul>

<ul>Why is React known as React
    <li>And it's called React because it reacts. It was developed by Facebook (a site that CONSTANTLY updates their
        data) to improve the user interface development and more effectively change (REACT to) what the user sees when
        they're doing things like mouse clicking, submitting and typing.</li>
</ul>

<ul>What is difference between react.development.js and react.production.js files via CDN
    <li>Development Environment: react.development.js Debugging Support: This file includes extra warnings and error
        messages to help developers identify and fix issues during development.

        Code Size: Larger file size due to the inclusion of development-specific tools and warnings.

        Performance: The development version is optimised for providing more helpful information and tools rather than
        being focused on minimal file size or performance. <br>

        Production Environment: react.production.js Minimised Code: This file is optimised for production use by
        removing development-specific warnings and tools, resulting in smaller file size.

        Performance: It is tuned for better runtime performance in production environments.

        Error Messages: Error messages are more concise, as the development-specific warnings are stripped away.</li>
</ul>

<ul>What is diference between React and ReactDOM
    <li>1. React:
        Let’s create reusable pieces of UI called components.
        Helps you build user interfaces (UIs) in JavaScript.
        Makes it easy to update and show UI changes based on data.
        <br>
        2. React DOM:
        Specifically deals with showing React components on web pages.
        Without ReactDOM, React wouldn’t know how to display things on a web page.
        Takes care of connecting your React code to the actual HTML on a webpage.

        In simple terms, React is like the architect who designs how things should look, and ReactDOM is the
        construction worker who puts those designs into action on a website. If you’re building web pages with React,
        you use both React and ReactDOM.
    </li>
</ul>

<ul>What is async and defer
    <li>Async -
        When we include a script with the async attribute, it tells the browser to download the script asynchronously
        while parsing the HTML document. The script is downloaded in the background without blocking the HTML parsing
        process.

        Once the script is downloaded, it's executed asynchronously, meaning it can run at any time, even before the
        HTML document has finished parsing.

        <!-- <script src="example.js" async></script> -->

        If multiple scripts are loaded asynchronously, they will execute as soon as they finish downloading, regardless
        of their order in the document. It is useful when the script doesn't depend on the DOM being fully loaded or
        other scripts.
    </li>
    <li>
        Defer -
        When we include a script with the defer attribute, it also tells the browser to download the script
        asynchronously while parsing the HTML document.
        However, the execution of the script is deferred until after the HTML document has been parsed.
        <!-- <script src="example.js" defer></script> -->
        Scripts with the defer attribute will execute in the order they appear in the document. It is useful when the
        script relies on the DOM being fully parsed or when script execution order is important.
    </li> <br>
    Conclusion
    Both async and defer allow the HTML parsing process to continue without waiting for the script to be downloaded.

    The difference lies in when the script is executed:
    With async, the script executes as soon as it's downloaded, potentially before the HTML document is fully parsed.
    With defer, the script executes only after the HTML document is fully parsed, but before the DOMContentLoaded event.

    One of the important things to note is, that we should only use async when we have scripts that can run
    independently and don't rely on the DOM structure, and we use defer when we need to maintain script execution order
    or depend on the DOM structure.
</ul>