# In Class Problem Set 3

I used ComboBoxDemo.java a few years ago.  It used to compile cleanly.  Even though the code has not changed, it now  will not compile without throwing warnings.

Doing everything from a command prompt or Git Bash (no IDEs allowed), your mission is to debug the code and find out why it stopped compiling cleanly.  When you have figured it out,  note what you changed and why it stopped working in the README.md file.

Name: Lexi Randt, Howard Li


**Changes to code**

static JComboBox cBox1 --> static JComoBox<String> cBox1 

cBox1 = new JComboBox(s) --> cBox1 = new JComboBox<String>(s)


**What caused it to stop working?**
JComboBox is a generic class JComboBox<E> where E is the type of items it holds, orignal program did not specify.
