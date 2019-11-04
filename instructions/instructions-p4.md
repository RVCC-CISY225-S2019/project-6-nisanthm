# Project 4
## Mobile First

**You must use our CSS formatting rules from the CISY 225 Style Guide.**

**You Must Have an Archived Project 3 Repo.**

 By making sure P3 is archived, you protect yourself from pushing changes to the wrong repo.

### Summary

You are going to have to clone the files from Project 3 into this repo.  You will be making new sizes of your three P3 gallery images and your "about me" profile picture to use in the picture element.  

Then you'll edit index.html and styles.css to make the required changes. 
  
See [Built-in Browser Support for Responsive Images](https://www.html5rocks.com/en/tutorials/responsive/picture-element/ "Built-in Browser Support for Responsive Images") for a cute demo.

### Instructions

1. Download this repo and the clone of your completed and Project 3 repo.

2. Copy P3 into P4 and delete the local copy of P3. (Make sure you do not copy the .git folder.)

3. Edit your README.md file to be about P4.

4. Delete everything in styles.css (make it an empty file) and save it.

5. Commit and push. Then check that it goes into the P4 GitHub repo. 

6. Find the large, original, versions of the 3 pictures that you used for P3 along with your personal "about me" image. All images, even 
your profile photo, need to be yours and not found on the Internet. If needed, find a new profile photo that is large enough.

7. Resize those large versions to the below specifications. You will end up with 16 files.

     | width  | filename addition |
     | ------------- | ------------- |
     | 1960px  | -1960w  |
     | 1024px  | -1024w  |
     | 640px  | -640w  |
     | 320px  | -320w  (The 3 gallery images are in P3. Add a 320px prolfile image.)|


8. Make sure these 16 pictures are in the `images` folder. You may make sub-folders in the `images` folder to help organize your pictures. Make sure the names of your sub-folders are lowercase and no spaces.

9. In the index.html file, for each of your three images and your "about me" profile image, replace the plain img element with a picture element that is properly set up for your images. It is very important to get the correct order of the `source` tags and to include
the `img` tag.
Here is an example. Showing:

The "about me" profile image.

```
<section class="hero">
  <h2>Hello, I'm</h2>
  <div class="content">
    <picture>
      <source media="(min-width: 1960px)" srcset="images/pix-me-1960w.jpg">
      <source media="(min-width: 1024px)" srcset="images/pix-me-1024w.jpg">
      <source media="(min-width: 640px)" srcset="images/pix-me-640.jpg">
      <img src="images/pix-me-320w.jpg" alt="This is a picture of me">
    </picture>
  </div>
</section>
```

And one of the Photo Gallery images.

```
<figure>
  <picture>
    <source media="(min-width: 1960px)" srcset="images/butterscotch-1960w.jpg">
    <source media="(min-width: 1024px)" srcset="images/butterscotch-1024w.jpg">
    <source media="(min-width: 640px)" srcset="images/butterscotch-640w.jpg">
    <img src="images/butterscotch-320pw.jpg" alt="My cat Butterscotch.">
  </picture>
  <figcaption>This is my beautiful Butterscotch!</figcaption>
</figure>
```

10. Using VS Code, edit the `logo-1913689.svg` file (do not edit `index.html`) and modify the existing line 12 to read, 

```
<svg width="52px" enable-background="new 0 0 520 520" version="1.1" viewBox="0 0 520 520" xml:space="preserve" xmlns="http://www.w3.org/2000/svg">
```

Pay close attention to your editing. It is the `width:"52px"` that you are adding to line 12 of the `logo-1913689.svg` file. Everything else stays the same.
Save, overwriting the `logo-1913689.svg` file.

11. Edit your empty styles.css file.

12. You are changing from a sans-serif font to a serif font. In the CSS, specify on the `body` element a font-family property with one Google font and one system font. Choose a serif font-family that has at least the 400, 400i, and 600 weights. Replace 'Fira Sans' in your `index.html` and `styles.css` files.

  Use this link https://fonts.google.com/?category=Serif&stylecount=6 to find a serif font.     
 
13. The CSS for each image should make the image have a max-width of 100%. You added this in P3. Add it again in P4. After this you will have only two, very simple, rules in your CSS. 

14. Commit and push P4 repo all of your edited files, making sure the pictures remain in the images folder on upload. 

15. Make sure your CSS code passes the CISY 225 Styleguide.

 * Use 2 spaces for indentation.
 * Put a space before the opening brace { in rule declarations.
 * In properties, put a space after, but not before, the colon : character.
 * Put closing braces } of rule declarations on a new line.
 * Put blank lines between rule declarations.
 * No spaces after the ; character.
 
16. Validate your html. **If your html does not pass validation, that is an immediate -3 points this assignment.**

17. Validate your CSS.  **If your CSS does not pass validation, that is an immediate -3 points on this assignment.**


