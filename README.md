How to Install OpenAI Gym in a Windows Environment?

Step 1: Install Microsoft Visual C++ Build Tools for Visual Studio 2017

Step 2: Install All Necessary Python Packages

      conda create -n gym python=3 pip

Step 3: Does a minimum install of OpenAI Gym

      pip install gym

Step 4: Install pystan; necessary to run the ToyText environments

      conda install pystan

Step 5: Install Atari environments

      conda install git
      pip install git+https://github.com/Kojoley/atari-py.git
      

Step 6: Install Box2D environments

      conda install swig
      pip install Box2D

Step 7: Installs the remaining OpenAI Gym environments

      pip install gym[all]

      Some errors may appear, but just ignore them.

Step 8: The last two lines are necessary to avoid some bugs that can occur with Pyglet and the Box2D environments.

      pip install pyglet==1.2.4
      pip install gym[box2d] 

Step 9:  Install Xming

Install Xming on your computer, which can be downloaded for free from:

      https://sourceforge.net/projects/xming/

Step 10: Start Xming Running

Each time you want to use OpenAI Gym, before starting your Python IDE, start Xming running by entering the following command at the Windows command prompt:

      set DISPLAY=:0

