# project_fileSearch
A python script that allows you to scrub a directory tree after specifying a directory and allows you to copy them all into a folder of your choosing.

INTRO:
- This started as a side project while I was taking an Intro To Python class at Western Oregon University. I love how simple it is to just throw something together using Python and this was the first time that I felt the confidnece to use programming to solve a personal problem. I had an iphone and I didn't like using ITunes to transfer the pictures and videos and so once I had done so they ended up in a very weird directory structure were I would dive three to four folders deep to get a couple pictures and some videos, then go two folders back up to check the others..and so on. This little script was written because I had a video I know that I had transfered and I couldnt find it because they were not named, they all had a default number assigned. The script simply takes a directory you specify and uses a module called 'shutil' and takes a specified file type, in this case it was '.mov' and collects all instances of it under that root directory. Then I created a new folder on my desktop on copied them all into it. From there I just went through them until I found what I wanted, crude, but in my mind it was a big accomplishment and because of the ease of Python and the available help with simple Google searches it didn't take long at all.

Installing:
- There's nothing fancy with any installation here, I am new to Python and this is a simple script that you can run by saving it, open a terminal and make sure your in the directory you saved the script in..type 'python fileSearch.py' to run it and follow the instructions.

- I suppose you should make sure to have Python installed.

Copyright:
    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

Credit:
- I very much want to give credit where it is due, a lot of code that I use I find through my searching on Google, there are a couple sources that I have referenced specifically in comments where I found a function to bring up a gui to choose a directory and return a string.
- http://stackoverflow.com/questions/25282883/how-can-i-use-the-output-from-tkfiledialog-askdirectory-to-fill-a-tkinter-entry
- I also did another search to figure out how to get rid of the gui once you have chosen a directory.
- https://www.daniweb.com/programming/software-development/threads/210657/open-directory-dialog-box

Modules:
- OS.walk() is what I use to dive into a directory
- Tkinter is the module used to provide the GUI associated with choosing a directory instead of typing the entire path like I started with.
- shutil is the module used in the copyfile() method, I found this after one easy search on stack overflow. 
