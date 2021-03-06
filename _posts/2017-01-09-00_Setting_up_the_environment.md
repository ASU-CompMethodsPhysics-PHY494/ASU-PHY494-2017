---
layout: post
title: 00 Installing the environment
---

----

Note: the course website is accessible at **https://goo.gl/bXs7NE**

----

The instructions were taken from [Software
Carpentry]({{site.swc_site}}), in particular [David
Dotson's recent workshop at
ASU](http://smallerthings.org/2016-01-07_asu_physics/).

## Overview

You will need to install

1. [The Bash Shell](#shell)
2. [Git](#git)
3. a [text editor](#editor) (by default, `nano`)
4. [Python](#python) (including a number of additional packages
required for scientific computing)

In each section, find the instructions for your operating system
(Windows, Mac OS X, or Linux).

Once you have installed everything, [test your
installation](#testing).


## Setup

<p>
  To participate in a the class, you will need
  access to the software described below. In addition, you will
  need an up-to-date web browser.
</p>
<p>
  SoftwareCarpentry maintains a list of common issues that occur during installation as a reference for instructors
  that may be useful on the
  <a href = "https://github.com/swcarpentry/workshop-template/wiki/Configuration-Problems-and-Solutions">Configuration Problems and Solutions wiki page</a>.
</p>

<div id="shell"> <!-- Start of 'shell' section. -->
  <h3>The Bash Shell</h3>

  <p>
    Bash is a commonly-used shell that gives you the power to do simple
    tasks more quickly.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="shell-windows">Windows</h4>
      <ol>
        <li>Download the Git for Windows <a href="https://git-for-windows.github.io/">installer</a>.</li>
        <li>Run the installer and follow the steps bellow:
          <ol>
            <!-- Git 2.6.1 Setup -->
            <!-- Welcome to the Git Setup Wizard -->
            <li>Click on "Next".</li>
            <!-- Information -->
            <li>Click on "Next".</li>
            <!-- Select Destination Location -->
            <li>Click on "Next".</li>
            <!-- Select Components -->
            <li>Click on "Next".</li>
            <!-- Select Start Menu Folder -->
            <li>Click on "Next".</li>
            <!-- Adjusting your PATH environment -->
            <li>
              <strong>
                Select "Use Git from the Windows Command Prompt" and click on "Next".
              </strong>
                If you forgot to do this programs that you need for the workshop will not work properly.
                If this happens rerun the installer and select the appropriate option.
            </li>
            <!-- Configuring the line ending conversions -->
            <li>
              Click on "Next".
              <strong>
                Keep "Checkout Windows-style, commit Unix-style line endings" selected.
              </strong>
            </li>
            <!-- Configuring the terminal emulator to use with Git Bash -->
            <li>
              <strong>
                Select "Use Windows' default console window" and click on "Next".
              </strong>
            </li>
            <!-- Configuring experimental performance tweaks -->
            <li>Click on "Next".</li>
            <!-- Installing -->
            <!-- Completing the Git Setup Wizard -->
            <li>Click on "Finish".</li>
          </ol>
        </li>
      </ol>
      <p>This will provide you with both Git and Bash in the Git Bash program.</p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">Mac OS X</h4>
      <p>
        The default shell in all versions of Mac OS X is Bash, so no
        need to install anything.  You access Bash from the Terminal
        (found in
        <code>/Applications/Utilities</code>). You may want to keep
        Terminal in your dock for this workshop.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        The default shell is usually Bash, but if your
        machine is set up differently you can run it by opening a
        terminal and typing <code>bash</code>.  There is no need to
        install anything.
      </p>
    </div>
  </div>
</div> <!-- End of 'shell' section. -->

<div id='git'> <!-- Start of 'Git' section. GitHub browser compatability
           is given at https://help.github.com/articles/supported-browsers/-->
  <h3>Git</h3>

  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported</a>
    web browser (current versions of Chrome, Firefox or Safari,
    or Internet Explorer version 9 or above).
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="git-windows">Windows</h4>
      <p>
        Git should be installed on your computer as part of your Bash
        install (described above).
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-macosx">Mac OS X</h4>
      <p>
        <strong>For OS X 10.9 and higher</strong>, install Git for Mac
        by downloading and running the most recent "mavericks" installer from
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
        After installing Git, there will not be anything in your <code>/Applications</code> folder,
        as Git is a command line program.
        <strong>For older versions of OS X (10.5-10.8)</strong> use the
        most recent available installer labelled "snow-leopard"
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-linux">Linux</h4>
      <p>
        If Git is not already available on your machine you can try to
        install it via your distro's package manager. For Debian/Ubuntu run
        <code>sudo apt-get install git</code> and for Fedora run
        <code>sudo yum install git</code>.
      </p>
    </div>
  </div>
</div> <!-- End of 'Git' section. -->

<div id="editor"> <!-- Start of 'editor' section. -->
  <h3>Text Editor</h3>

  <p>
    When you're writing code, it's nice to have a text editor that is
    optimized for writing code, with features like automatic
    color-coding of key words.  The default text editor on Mac OS X and
    Linux is usually set to Vim, which is not famous for being
    intuitive.  if you accidentally find yourself stuck in it, try
    typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q',
    exclamation mark), then hitting Return to return to the shell.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="editor-windows">Windows</h4>
      <p>
        nano is a basic editor and the default that is used in the class.
        To install it,
        download the <a href="{{site.swc_installer}}">Software Carpentry Windows installer</a>
        and double click on the file to run it.
        <strong>This installer requires an active internet connection.</strong>
      </p>
      <p>
        Others editors that you can use are
        <a href="http://notepad-plus-plus.org/">Notepad++</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>, <a href="https://atom.io/">Atom</a>.
        <strong>Be aware that you must
          add its installation directory to your system path.</strong>
        Please ask your instructor to help you do this.
      </p>
      </div>
    <div class="col-md-4">
	<h4 id="editor-windows-asu">Windows (on ASU laptop without superuser
      privileges)</h4>
	  
      <p>On the ASU school laptops, <b>Sublime Text 3</b> is pre-installed
    and you can use it instead of <tt>nano</tt> (which cannot be installed
    without superuser privileges). Launch the editor from the Start Menu.
    </p>
	
	<p>Customize the PATH environment so that you can launch
    <tt>sublime_text.exe</tt> from the command line:</p>
	<ol>
		<li>Open the Git-Bash command line</li>
		<li>Create the file <tt>$HOME/.bash_profile</tt> with the following content by typing
		<pre>
cat > $HOME/.bash_profile << 'EOF'
# PHY494 bash startup
export PATH="/c/Program Files/Sublime Text 3/:$PATH"
EOF
</pre>This will instruct Bash to look for your sublime text
editor.</li>
    </ol>
    </div>

    <div class="col-md-4">
      <h4 id="editor-macosx">Mac OS X</h4>
      <p>
        nano is a basic editor and the default that instructors use in the workshop.
        It should be pre-installed.
      </p>
      <p>
        Others editors that you can use are
        <a href="http://www.barebones.com/products/textwrangler/">Text Wrangler</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>, <a href="https://atom.io/">Atom</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="editor-linux">Linux</h4>
      <p>
        nano is a basic editor and the default that instructors use in the workshop.
        It should be pre-installed.
      </p>
      <p>
        Others editors that you can use are
        <a href="https://wiki.gnome.org/Apps/Gedit">Gedit</a>,
        <a href="http://kate-editor.org/">Kate</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>, <a href="https://atom.io/">Atom</a>.
      </p>
    </div>
  </div>
</div> <!-- End of 'editor' section. -->

<div id="python"> <!-- Start of 'Python' section. Remove the third paragraph if
           the workshop will teach Python using something other than
           the IPython notebook.
           Details at http://ipython.org/ipython-doc/2/install/install.html#browser-compatibility -->
  <h3>Python</h3>

  <p>
    <a href="http://python.org">Python</a> is a popular language for
    scientific computing, and great for general-purpose programming as
    well.  Installing all of its scientific packages individually can be
    a bit difficult, so we recommend
    <a href="https://www.continuum.io/anaconda">Anaconda</a>,
    an all-in-one installer.
  </p>

    <p>
      Regardless of how you choose to install it,
      <strong>please make sure you install Python version 3.x</strong>
      (e.g., 3.4 or 3.5 is fine).
    </p>

    <p>
      We will teach Python using the Jupyter notebook, a programming environment
      that runs in a web browser. For this to work you will need a reasonably
      up-to-date browser. The current versions of the Chrome, Safari and
      Firefox browsers are all <a
      href='http://ipython.org/ipython-doc/2/install/install.html#browser-compatibility'>supported</a>
      (some older browsers, including Internet Explorer version 9
      and below, are not).
      </p>

<div class="row">

    <div class="col-md-4">
      <h4 id="python-windows">Windows</h4>
      <ol>
        <li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
        <li>Download the Python 3 installer for Windows.</li>
        <li>Install Python 3 using all of the defaults for installation <em>except</em> make sure to check <strong>Make Anaconda the default Python</strong>.</li>
      </ol>
    </div>

    <div class="col-md-4">
      <h4 id="python-windows-asu">Windows (on ASU laptops without
      sysadmin and existing system anaconda)</h4>
	  <p>If you are stuck with a laptop where you can only install as
    a user <em>and</em> there is already a system-wide anaconda installation
    present then you will need to install your own anaconda <em>and</em> make
    sure that it is being used.</p>
      <ol>
        <li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
        <li>Download the Python 3 installer for Windows.</li>
        <li>Install Python 3 using all of the defaults for
    installation <em>except</em> make sure to check <strong>Make
    Anaconda the default Python</strong>.</li>
		<li>Open the Git-Bash command line</li>
		<li>Append (<tt>>></tt>) to the file <tt>$HOME/.bash_profile</tt> the following content by typing
		<pre>
cat >> $HOME/.bash_profile << 'EOF'
# PHY494 bash startup for local Anaconda
MYCONDA="$HOME/Anaconda3"
export PATH="$MYCONDA:$MYCONDA/Scripts:$MYCONDA/libs/bin:$PATH"
unset MYCONDA
EOF
</pre>This will instruct Bash to look for your conda installation
before anything else.</li>
    <li>Close the Git-Bash window.</li>
	<li>Open a new Git-Bash window (so that your changes take effect).</li>
    </ol>
    </div>

    <div class="col-md-4">
      <h4 id="python-macosx">Mac OS X</h4>
      <ol>
        <li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
        <li>Download the Python 3 installer for OS X.</li>
        <li>Install Python 3 using all of the defaults for
		installation.</li>
      </ol>
      </div>
	  
    <div class="col-md-4">
      <h4 id="python-linux">Linux</h4>
      <ol>
        <li>Open <a href="http://continuum.io/downloads">http://continuum.io/downloads</a> with your web browser.</li>
        <li>Download the Python 3 installer for Linux.</li>
        <li>Install Python 3 using all of the defaults for installation.
        (Installation requires using the shell. If you aren't
        comfortable doing the installation yourself
        stop here and request help.)</li>
        <li>
          Open a terminal window.
        </li>
        <li>
          Type <pre>bash Anaconda-</pre> and then press
          tab. The name of the file you just downloaded should
          appear.
        </li>
        <li>
          Press enter. You will follow the text-only prompts.  When
          there is a colon at the bottom of the screen press the down
          arrow to move down through the text. Type <code>yes</code> and
          press enter to approve the license. Press enter to approve the
          default location for the files. Type <code>yes</code> and
          press enter to prepend Anaconda to your <code>PATH</code>
          (this makes the Anaconda distribution the default Python).
        </li>
      </ol>
    </div>

</div> <!-- End of 'Python' section. -->


  <h3>VPython</h3>

<p>For 3D visualization, we will use Jupyter <a href="http://vpython.org/">vpython</a> within the Jupyter notebook
interface. This is not part of anaconda and so we need to install it separately after the anaconda installation.
</p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="vpython-windows">Windows</h4>
      <ol>
        <li>Open the git-bash shell commandline (Start Menu: All
    Programs: Git: Git Bash)</li>
    <li>Type in the command line
	<pre>pip install vpython</pre>
	</li>
    </ol>
    </div>
    <div class="col-md-4">
      <h4 id="vpython-macosx">Mac OS X</h4>
      <ol>
      <li>Open the Terminal (command line)</li>
      <li>Type
         <pre>pip install vpython</pre>
	   </li>
      </ol>
    </div>
    <div class="col-md-4">
      <h4 id="vpython-linux">Linux</h4>
      <ol>
	   <li>Open the Terminal (command line)</li>
            <li>Type <pre>pip install vpython</pre></li>
      </ol>
    </div>
  </div> <!-- End of 'VPython' section. -->
</div>



## Testing

### Bash shell

Open a *terminal* (Mac OS X, Linux) or open *Git Bash* (under
*All Programs/Git/Git Bash*) in Windows.

Type

{% highlight bash %}
echo $SHELL
{% endhighlight %}

Should show `/bin/bash` or `/usr/bin/bash` (or similar).

We use "shell" and "terminal" (and "console") pretty
interchangeably.

### Git

In the shell, type

{% highlight bash %}
git --version
{% endhighlight %}

which should show something like `git version 2.7.0`.

### nano

In the shell, type

{% highlight bash %}
nano
{% endhighlight %}

You should see `GNU nano 2.0.6` (or similar in the top line) and at
the bottom of the screen `^X Exit     ^J Justify` (and more). Quit
nano by holding down the `control` key together with `X`,
i.e. `control + X`. In Unix keystrokes, the control key is typically
indicated with the caret character `^`.

(If you don't have `nano` but some other editor such as `Sublime Text`
check the section on <a href="#editor-windows-asu">Editor under
Windows (ASU)</a> and ask an instructor for help.)

### Python

In the shell, type

{% highlight bash %}
python -c 'import sys; print(sys.version)'
{% endhighlight %}

which should give something similar to `3.5.2 |Anaconda 4.2.0
(64-bit); (default, Jul  2 2016, 17:53:06)` (and more
stuff). Important: you should have *Python 3*, i.e., a version like
3.4.x or 3.5.x.



### Jupyter notebook and VPython

<ol>
<li>
In the shell, type

{% highlight bash %}
jupyter notebook
{% endhighlight %}

This should open a browser window at <a href="http://localhost:8888">http://localhost:8888</a>. 
</li>
<li>Open the <tt>New</tt> menu on the right hand side.</li>
<li>Under <tt>Notebooks</tt> select <tt>Python [conda root]</tt></li>
<li>In the new window ("Untitled"), type
{% highlight python %}
print("Hello World!")
{% endhighlight %}
and press <tt>shift</tt> and <tt>return</tt> keys simultaneously to evaluate the
cell. It should print "Hello World!".</li>
<li>Close the browser tab with menu <tt>File: Close and Halt</tt>.</li>
<li>In the files listing, select from <tt>New</tt> under <tt>Notebooks</tt> select
<tt>VPython</tt></li>
<li>In the new window ("Untitled2"), type
{% highlight python %}
import vpython as vp
box = vp.box()
{% endhighlight %}
and press <tt>shift</tt> and <tt>return</tt> keys simultaneously to evaluate the
cell. It should open a graphics window in the notebook showing a
cube. Use the mouse with right mouse button presse to turn the cube
(on Mac OS X, press <tt>control</tt> while clicking/pressing the touch pad to
get "right click").</li>
<li>Close the browser tab with menu <tt>File: Close and Halt</tt>.</li>
</ol>

<p>
If you have problems, ask an instructor.
</p>


#### Common problems

* On Mac OS X, if you get the error *OSError: [Errno 49] Can't assign
  requested address* you might need to use `jupyter notebook
  --ip=127.0.0.1`
* Wrong `conda` is used. Check `which conda` in the terminal: it
  should show a path in your home directory (e.g., for user "physics":
  Windows: `/c/Users/Physics/Anaconda3/conda`, Mac OS X:
  `/Users/physics/Anaconda3/conda`, Linux:
  `/home/physics/Anaconda3/conda`). Try exiting the terminal and open
  a new terminal (or git bash) and try again. Changes to PATH only
  take effect when a new shell is opened.
* The spinning box in VPython is not visible, only a blank square. Try
  opening the notebook in the Chrome web browser instead of
  Explorer/Edge: Just type `http://localhost:8888` in Chrome's URL bar.
