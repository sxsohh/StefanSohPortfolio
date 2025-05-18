# Stefan Soh's Portfolio

![image](https://media.licdn.com/dms/image/v2/D5603AQF5e0H3s1zakQ/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1722352828141?e=1753315200&v=beta&t=750HXGWXYMt_TEPYBxYTXuaD39yfSO_dW-n59olkfM8)

## Table of Contents
- **External Links**
  ```yaml
      linkedin:       # https://www.linkedin.com/in/stefanxsoh/ 
      github:         # https://github.com/sxsohh 
  ```


- **Skills**:
    ```yaml
      skills:
        - category: Technical
          - Python
          - Data Structures & Algorithms: Understanding of arrays, linked lists, stacks, queues, trees, recursion, and sorting algorithms
          - Data Analysis: Ability to collect, clean, transform, and analyze datasets
          - Data Visualization: Experience generating visual insights using open-source tools (matplotlib) 
        
        - category: Analytical/Research
          - Impact Evaluation: Measuring program effectiveness (Move For Hunger)
          - Comparative Financial Analysis: Comparing returns and creating performance benchmarks (Cannataro internship)
          - Problem Solving: Designing and debugging algorithms and visual data narratives
          - Partnership Research: Outreach and stakeholder mapping

        - category: Soft Skills
          - Collaboration & Teamwork: Frequent hands-on group projects and community engagement
          - Time Management: Balanced rigorous academics, basketball, and multiple internships
          - Communication: Comfortable presenting findings through both writing and public speaking
          - Adaptability: Worked in diverse settings — from nonprofit teams to finance environments
    ```
- **Contact Form**: you can set up the contact form to send the response to your email using [formspree](https://formspree.io/). You just need to sign up and create a new form. Then, add the 8-digit endpoint key!
 
  ![formspreeimage](/assets/readme/formspree.png)

  ```yaml
  formspree-key:   https://formspree.io/f/{8-digit key}
  ```

- **(optional)** you chan change your color theme by inputting color hex code for a few variables. Feel free to be creative!
  ```yaml
  colors: # this is the basic theme
    text: "##1a1c20"
    border: "#ddd"
    link: "#4a76ee"
    highlight: "#0c0cf2"
    background: "#ffffff"
    light_background: "#f3f5fb"
  ```
  There is a few suggested themes in `_config.yml`
  - **mint green**
  ![GitHub Use Template](/assets/readme/mint-green.png) 
  - **lemon**
  ![GitHub Use Template](/assets/readme/lemon.png) 
  - **cotton-candy**
  ![GitHub Use Template](/assets/readme/cotton-candy.png) 

## Adding projects
For each project, you need to create a markdown file within _projects folder. I recommend created a folder for each project so that it is easy to organize image files that you may want to add. To get started, follow the below steps.

#### Creating a markdown file in Github
1. Go to **_project** folder. Make sure you are in the correct level.
![GitHub Use Template](/assets/readme/go-to-project-directory.png) 
2. In the right side of the screen, click add file - create new file.  
![GitHub Use Template](/assets/readme/create-new-file.png) 
3. in the available field, enter the name of the folder: **{your-project-name}** then hit "/". This will create a folder for the project.   
![GitHub Use Template](/assets/readme/enter-folder-name.png) 
4. create a markdown file by entering index.md.   
![GitHub Use Template](/assets/readme/index-md.png) 
5. In the text field paste the below "front-matter" template and fill out the title, description, skills, and name of the main project image that you want to use. This is the summary of the project that will be used to display the project in the main page. **Be careful** not to leave any space before the front matter deliminators "---". It causes syntax error, and  your page will not be built.

    ```md
    ---
    layout: post
    title: project title
    description:  short description of the project
    skills: 
    - skill 1
    - skill 2
    main-image: /project.webp 
    ---
    ```
6. then click **Submit changes** to create the file.
7. Upload your image in the same folder by clicking **Add file - upload files**.
  
![GitHub Use Template](/assets/readme/create-new-file.png) 

8. Drag your image file, then click **commit changes**.
    
![GitHub Use Template](/assets/readme/upload-files.png) 

9. Allow a minute or so for the build. It will create a project section that looks like this below.
![GitHub Use Template](/assets/readme/project-section.png) 

### Understanding markdown file your project page
If you want to add addtional details, you can go back to the index.md file and add more contents below the front matter. It will be helpful if you become familiarized with markdown syntax. If you are interested in learning, see [markdown guide](https://www.markdownguide.org/cheat-sheet/). I set up a couple styling to allow you to embed multiple images and video easily and become responsive for mobile view. See the [demo](https://leea12.github.io/)) project. You can also add code blocks, blockquote, and tables. 

#### YAML frontmatter
YAML frontmatter gets pulled by the site to fill contents for the summary section of your project which gets displayed in the main index page and top section of the project page. 

```markdown
---
layout: post
title: Super Heavy Booster Catch (Demo Only)
description:  (I have never been employed by / affiliated with SpaceX. This is for demo use only) 
    Developing the Super Heavy booster catch project involves designing a robust launch tower with "chopstick" arms, advanced control systems for precise booster alignment, and integrating sophisticated software for real-time trajectory adjustments and structural engineering to handle immense forces.
skills: 
  - Structural analysis
  - Aerodynamic design
  - Propulsion system integration
  - Control Algorithem 
  - Welding
  - Metal forming
  - Thermal simulation

main-image: /project2.jpg
---
```
#### Adding contents
use "## (title)" as the title of each section
## Section title
```markdown
## section title
```

### sub-section title
Use this to have subsection if needed
```markdown
### sub-section title
```

#### Adding a new line
you can add 2 spaces "  " or <br> to start a new line
```markdown
<br>
```

#### Adding a horizontal line
you can add a horizontal line to separate fields by using "---"
```markdown
---
```

#### Embedding images 
Add images using the following format. You can put multiple images in a single row by putting in multiple entries for "images=". You can also overide the size of the all images in the single row setting the height in pixel.
{% include image-gallery.html images="{image1 path}, {image2 path}" height="400"%}

```markdown
{% include image-gallery.html images="project2.jpg" height="400" %}
```
#### Embedding youtube video
Add youtube video using the following format
{% include youtube-video.html id="{11-digit id}" autoplay= "false"%}
```markdown
{% include youtube-video.html id="{11-digit id}" autoplay= "false"%}
```
This is where you get the 11-digit id  

![image](https://github.com/user-attachments/assets/4ffc509a-9e22-40bc-b503-421443ab2b66)

#### Adding bold text
add bold text by wrapping with "**"
```markdown
this is how you input **bold text**
```

#### Adding italic text
add italic text by wrapping with "*"
```markdown
Italicized text is the *cat's meow*.
```

### adding underline
underline is not supported in markdown, but you can still use html within markdown
```
<u>This text is underlined</u>
```

#### Adding ordered list
```markdown
1. First item
2. Second item
3. Third item
4. Fourth item
```
1. First item
2. Second item
3. Third item
4. Fourth item

#### Adding unordered list
```markdown
- First item
- Second item
- Third item
- Fourth item
```
- First item
- Second item
- Third item
- Fourth item

#### Adding code block
To add a code block wrap your script with ```. Adding the language after ''' will activate sytax highlighting.
![image](https://github.com/user-attachments/assets/8b8a6c6a-1599-4b03-bcc3-b087bc0f5c49)

```python
def start()
  print("time to start!")
```

#### Adding external links
to add extra links, wrap the text in "[ ]" then add the add the hyperlink wrappted by "( )"
```markdown
[Wikipedia](https://en.wikipedia.org)
```
#### Adding block quote
To add a blockquote add ">" at the beginning of the text
```markdown
> A blockquote would look great if you need to highlight something
```
> A blockquote would look great if you need to highlight something

#### Adding table
To add a table, use the following format
```markdown
| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |
```
| Header 1 | Header 2 |
|----------|----------|
| Row 1, Col 1 | Row 1, Col 2 |
| Row 2, Col 1 | Row 2, Col 2 |

** make sure to leave a line betwen the table and the header

