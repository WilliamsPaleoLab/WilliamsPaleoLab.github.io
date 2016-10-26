### Welcome to the Williams Lab Website Codebase

#### Adding a News Post
  1.  Go to the ```_posts``` folder
  2.  Create a new markdown document called ***YYYY-mm-dd-some-name.md***. The name must contain the date of the post and a short description of what its about.
  3.  Put a yaml header in the top of the document.  The header should contain:
    - ```layout: post```
    - ```title: [your title goes here]```
    - ```date: [date of post in format YYYY-mm-dd hh:mm:sss]```
    - ```categories: [a category of your choice]```.  This can be useful later for categorizing news posts when we have a whole bunch.
  4.  Write a markdown news post.  A good length is one to two sentences.  This post can contain photos and links, lists, quotes, etc.
  5.  Save the markdown file.
  6.  Run ```jekyll build```
  7.  Commit your changes.
  
#### Adding a Bio
  1.  Go to the ```_people``` folder.
  2.  Create a new markdown document called ***[personName].md***. 
  3. Go to the ```img/bio_img``` folder. Put an image of the person here, called ```personName.jpg```.  Any photo format is accepted.
  4.  Write a YAML header for the document. It should contain:
    - ```name: The person's name```
    - ```biography: A description of the person's interests and position.```
    -``` role: The role in the lab.``` Accepted values are "Professor", "Postdoc", "Graduate Student", "Undergraduate".  Sorry Simon, Research Scientist isn't an accepted value.  Currently, the role is only used for sorting and partitioning on the page.
    - ```linkedin: Link to linked in profile```
    -``` twitter: Link to twitter profile```
    - ```email: Email address```
    - ```orcid: Link to ORCID profile```
    - ```photo: "name of photo in bio_img folder".```  This should exactly match the name of the image you put in the ```img/bio_img```
    - ```seniority: A number representing how to sort.```  Categories (```role```s) will be partitioned and then sorted by  ```seniority```.
  5.  No markdown needs to be written in this file.  All bio information should go into ```biography``` key in YAML.
  6.  Save the file.
  7.  Run ```jekyll build```
  8.  Commit your changes.
  
