# Host Resume
The purpose of this readme is to create a simple pipeline to host a website. Anything could be hosted but we will host a resume. This project will use the modern approach as described by Andrew Etter in the book Modern Technical Writing, which is to use a lightweight markup language, format the document using a static site generator, and host the document on a distributed version control system. 

## Prerequisites

    A resume written in markdown

## Getting Started

### Distributed Version Control System
Using a distributed version control system is usefull for many reasons, but a few important ones are: automatic backups, offline work, easier for multiple people to contribute, and for automatic updating our website. We will use Github for our project because then we can also automatically host our resume with a few simple steps and the website will automatically update when we make changes. Etter stresses that when changes are made, the update process should be very simple because frequent updates are often necessary. 

1. [Click](https://github.com/login) to create Github Account

2. Create New Repository
    1. Click ```Create repository```
    2. Name the respository ```username.github.io``` This will ensure that the website will host automatically
    3. Click ```Create repository``` to save the changes

### Lightweight Markup Language
Now that the project is created it is time to upload the markdown resume. The reason we use markdown to create the resume is because markdown is flexible. It makes creating website content easy, it is human readable, it is platform independent, and are easy to use with static site generators. It doesn't do styling because that is done with a static site generator. This way we can edit markdown on any platform we're on and we're also not restricted to a fancy word processor.

3. Upload Resume
    1. Click ```uploading an existing file``` under the code section to upload your resume in markdown
    2. Rename the uploaded resume ```index.md``` so that github pages will use it for our website
    3. Add the following to the top of your resume

            ---
            title: Your Name
            ---
    4. Click ```Commit changes```

### Static Site Generator
Now that we have a markdown file, we're ready to apply a style to the resume and create a website out of it. By using markdown only for text makes it very easy to now apply any style to it that we like. This way we can edit the text independent of what style we use and vice versa. We will use Jekyll for our site generator because it is already integrated with github pages. There are many themes available, but I would start with [these](https://pages.github.com/themes/) themes that are already supported by github pages. For my resume I used the Cayman theme as can be seen by the following instructions. 

4. Create ```_config.yaml``` file
    1. Click ```Add file``` under the Code section
    2. Name the file ```_config.yaml```
    3. Add ```theme: jekyll-theme-cayman``` to the first line
    4. Click ```Commit changes```

### Site Complete
Congratulations! Your site should now be visible at ```username.github.io```. You might not see it immediately because it takes a minute or two to build and refresh the website. We have now created a complete pipeline to host a resume written in markdown and generated a static website with Jekyll. This is called a pipeline because you can now make a change to your resume or to the _config file and once you commit that change it will update the website for you automatically. That is the beauty of this modern approach and as you can imagine if there are multiple contributors working in different areas they can all commit changes whenever they like and the website just builds and deploys automatically. This is very different from where you used to dread making a change and updating documents in many different places and often with specialized software that only a few people know how to use. Additionaly, Github might be new to you but any experienced software developer know how to use a flavour of github. 

## More Resources
## Authors and Acknowledgements
## FAQs
1. Why is Markdown better than a word processor?
2. Why is my resume not showing up?