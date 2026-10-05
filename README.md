🖼️ I Frame – Assignment Navigation

A simple HTML and CSS project that uses an "<iframe>" to display multiple assignments within the same webpage.

The project provides a navigation panel on the left side. Clicking an assignment opens its corresponding HTML page inside the iframe on the right side without leaving the main page.

📸 Project Overview

The webpage is divided into two sections:

- Left Section: Contains buttons/links for Assignment 1 to Assignment 10.
- Right Section: Contains an "<iframe>" where the selected assignment is displayed.

Layout

┌─────────────────────────────────────────────────────────┐
│                    I Frame                              │
├───────────────────┬─────────────────────────────────────┤
│                   │                                     │
│   Assignment 1    │                                     │
│   Assignment 2    │                                     │
│   Assignment 3    │                                     │
│   Assignment 4    │                                     │
│   Assignment 5    │          Assignment Preview         │
│   Assignment 6    │             (iframe)               │
│   Assignment 7    │                                     │
│   Assignment 8    │                                     │
│   Assignment 9    │                                     │
│   Assignment 10   │                                     │
│                   │                                     │
└───────────────────┴─────────────────────────────────────┘

🛠️ Technologies Used

- HTML5
- CSS3
- HTML "<iframe>"

No external libraries or frameworks are required.

📂 Project Structure

iframe-project/
│
├── index.html
├── asaigmant1.html
├── news paper assignment 2.html
├── assignment3.html
├── assignment4.html
├── assignment 5.html
├── Home.html
├── Ananya and Yukta assignment 7.html
├── Assignement 8.html
├── Assignment 9 box plotting.html
├── Login.html
└── README.md

«The filenames above are based on the links used in the provided HTML code.»

🔗 Assignment Navigation

Each assignment is connected using an anchor ("<a>") element.

For example:

<div class="button">
    <a href="asaigmant1.html" target="box">Assignment1</a>
</div>

The important part is:

target="box"

The "target" attribute tells the browser to open the linked page inside the iframe whose "name" is "box".

🖼️ IFrame

The iframe is created using:

<iframe
    src=""
    frameborder="0"
    height="100%"
    width="100%"
    name="box">
</iframe>

The iframe occupies the complete right section of the container.

When an assignment link is clicked, its webpage is loaded into this iframe.

🎨 CSS Features

Main Container

.con {
    height: 600px;
    border: 1px solid black;
    display: flex;
}

The "display: flex" property places the navigation and iframe sections side by side.

Left Navigation

.left {
    height: 100%;
    width: 30%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    border: 1px solid black;
}

The left section takes 30% of the available width.

The assignment buttons are arranged vertically with equal spacing.

Right Section

.right {
    height: 100%;
    width: 70%;
    border: 1px solid black;
}

The right section takes 70% of the available width and contains the iframe.

Assignment Buttons

.button {
    height: 8%;
    width: 90%;
    border: 1px solid black;
    border-radius: 30px;
    text-align: center;
    line-height: 40px;
    background-color: antiquewhite;
}

The buttons have:

- Rounded corners
- Border
- Centered text
- Antiquewhite background
- 90% width of the navigation area

▶️ How to Run

1. Create a folder for the project.
2. Save the main HTML file inside the folder.
3. Place all assignment HTML files in the same folder.
4. Make sure the filenames match the "href" values exactly.
5. Open the main HTML file in a web browser.
6. Click an assignment button.
7. The selected assignment will appear in the iframe.

🎯 Learning Objectives

This project helps beginners understand:

- HTML links
- "<iframe>"
- "target" attributes
- Flexbox
- "display: flex"
- "flex-direction"
- "justify-content"
- Width and height
- Borders and border radius
- Basic webpage layout
- Linking multiple HTML pages together

💡 How It Works

The navigation link:

<a href="assignment3.html" target="box">
    Assignment3
</a>

points to:

<iframe name="box"></iframe>

When the link is clicked, "assignment3.html" is loaded into the iframe instead of opening a new page.

🚀 Possible Improvements

The project could be improved by:

- Adding hover effects to the assignment buttons
- Adding active button styling
- Making the layout responsive for mobile devices
- Removing the deprecated "frameborder" attribute and using CSS instead
- Adding a default assignment in the iframe
- Adding icons to the navigation buttons
- Using cleaner and consistent filenames
- Adding a home/reset button

👨‍💻 Author

Created as a beginner-friendly HTML, CSS, and iframe navigation project for practicing webpage linking and layout design.# I-frame
