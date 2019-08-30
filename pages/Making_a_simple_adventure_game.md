## Summary

 For a HTML stream, CoderDojo Tokyo uses a course that
creates a simple adventure game with kids, which automatically deployed
to servers via Dropbox. The article shows you how to prepare and how to
teach in the course. 

## Tips for use

You will need to either install Scratch on the
[Ninja](Ninja.md)'s machine or use the [web-based
editor](https://scratch.mit.edu/) in advance of using these cards.

## Content

### How to prepare

#### Pre-requisite for attendees

1.  Install and setup [Dropbox](https://www.dropbox.com/home) account.
    (if parents are already Dropbox users, use that account.)
2.  Tell the account(e-mail address) to his/her mentor.
3.  Install one of the following text editors.
      - Mac :
        [CotEditor](http://sourceforge.jp/projects/coteditor/releases/)
      - Win :
        [EmEditor](http://jp.emeditor.com/modules/download2/rewrite/tc_5.html)

#### Pre-requisite for mentors

1.  Signup Dropbox with your official account such as
    'tokyo@coderdojo.com'.
2.  Create 'html' directory in Dropbox folder, and add personal
    directory to the 'html'. (e.g. Dropbox/html/cognitom/)
3.  Share the personal directory with the attendee by e-mail address
    registered in Dropbox.
4.  If you want to use images, create 'image' directory and share it
    with attendees as well.
5.  [Download
    'shimokita'](https://github.com/coderdojo-tokyo/shimokita/zipball/template),
    and unzip it.

#### Dropbox-synced server

  - [Compile and install Dropbox](https://www.dropbox.com/help/247) on
    your Web server.
  - Create symbolic link of './Dropbox' to the root directory (e.g.
    /var/www/) and type '$ chmod 755 Dropbox' to be shared on the web.
  - Finally, check if 'Dropbox/html/' directory is able to be seen at
    your Web server.
  - NOTE: Because this system automatically publishes your works, make
    sure you don't add any secret data to the dropbox-synced directory.

### How to teach

1.  Create an account at [CodeAcademy](http://www.codecademy.com/).
2.  Follow HTML Fundamental course with kids. (you can pause and resume
    at any section if needed.)
3.  If finished courses, create HTML code in your local computer and
    check if it works on your web browser.
4.  Show and play Shimo-kitazawa Adventure as a sample web game, which
    uses the tags just you learned, such as 'p', 'img', and 'a' tags.
5.  Now, look at how it works by download and open 'index.html' with
    your editor.
6.  Comment out 'STYLE' tag to enable Style, then see if the style is
    changed.
7.  Show how to copy existing pages and to add pages.
8.  Show how to change images and sentences.
9.  Then, extend the game or create a game as you want; for example:
      - Add a 'Game Over' page with several patterns.
      - Take a picture and add it to the page.
      - Add a link to other kid's page.

### Reference

  - Sample Game : <http://tokyo.coderdojo.com/html/cognitom/>
  - Source Code
      - Master branch : <https://github.com/coderdojo-tokyo/shimokita>
      - Template branch:
        <https://github.com/coderdojo-tokyo/shimokita/tree/template>
