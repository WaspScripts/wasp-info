Title: Setup (Windows)
Description: Full installation setup of Simba, SRL, WaspLib and Scripts
Level: 0
Author: e40dee47-eb0c-4859-8434-44dd4d979673
Co-Authors:

# Video Setup

Video guide by @Daxious




### Downloads

You can download Simba from [**here**](https://github.com/Villavu/Simba/releases/download/simba1400-release/Simba-Win32.exe).

If for some reason that link is broken, you can see all Simba releases [**here**](https://github.com/Villavu/Simba/releases).
In this case, make sure you get the latest **32bits version**.
If you are on windows it's **very important** you use the **32bits** version of Simba.

### Setting up

To use Simba you pretty much only need to run it. However, since Simba needs to create some files and folders to work, I recommend you make a folder for it. For simplicity sake you can name it "Simba" and then put your Simba.exe in that folder.
![simba directory](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img00.png)

Now you are ready to run it!
Depending on where you placed your Simba.exe, the first time you run it you might get a warning from **Windows Defender SmartScreen** like this:
![warning 1](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img01.png)
Click "**More info**".
![warning 2](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img02.png)
And then "**Run anyway**".

Wait for Simba to open up...

Once it opens for the first time, you can **optionally associate simba scripts with simba**:
![associate scripts](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img03.png)

It doesn't really matter what you choose... I choose Yes.

Now you can also **optionally** disable the command line prompt.
I personally find it annoying when I don't need it.
![img04](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img04.png)

You can minimize or close Simba for now.

If you check your Simba folder now you will see it has a bunch of new stuff there:
![img05](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img05.png)

In there you will find 2 important folders: **Includes** and **Scripts**.

The Includes folders is where you will put the **Includes** (well duh...).

An include is a sort of framework, a **collection of common functions and procedures** so scripts don't have to contain everything.
Examples of includes are SRL and my WaspLib.
You might not need to use this folder though since Simba has a tool to setup things automatically for us.

The Scripts folder is where you will put the scripts you download or **create**.

Now we are going to install SRL-T and WaspLib.
You have 3 ways of installing includes, manual,  automatically through Simba or using git.

To manually install a Include, simply download it's zip file from github, and unzip it in:

```cmd
C:\Simba\Includes\
```
You can download SRL-T from here:
> https://github.com/Torwent/SRL-T

Unzip it, change it's name to whatever is required, for example if your unzipped folder is named "SRL-T-master", rename it to "SRL-T" and place it in Includes.

Using git is similar to the manual install, but with git. If you are using it I'm going to assume you don't need instructions.

For the automatic install which I recommend for most people, open up Simba and click on the package 📦️ icon.

![img06](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img06.png)

In the window that opens up, click the plus icon in the top left corner.

![img07](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img07.png)

Paste the link of the include you want to install...

![img08](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img08.png)

Click **Ok** and then click **Install**

If you get prompted with a overwriting warning click **Yes**.

Once that is done, you can install **WaspLib** the same way.

The link to **WaspLib** is:

> https://github.com/Torwent/WaspLib

Press the **plus icon**, paste the **link** above, click **Ok** and click **Install**.

You can close the **package manager** now.

Now we are going to test if everything was setup correctly.

Type this code into Simba:

```pascal
{$I SRL-T/osr.simba}
{$I WaspLib/osr.simba}
```

Open your **Old School RuneScape Client** and let it load up to the Login Screen.

If you are on **Windows**, I strongly recommend you use the **Official OSRS Client** (not the new steam one).

**RuneLite is not supported!**

Once that's done, **click and drag the green crosshair** on Simba to your RuneScape Client.

![img09](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img09.png)

You will see the windows you drag the crosshair through being highlighted, once the RuneScape client is highlighted release the mouse.
Keep in mind you should only select the client and nothing of the border.

In this case this first example is **wrong**:

![img10](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img10.png)

This one is **right**:

![img11](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img11.png)

Doing this tells Simba that will be it's **target**, because in reality **you can use Simba for other things** that are not RuneScape.

Once you set your client as your target, click the green arrow.
That's the **Play button** for all scripts.

![img12](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img12.png)

The script will run and if everything is working properly, the output on your debugger should be something similar to this:

![img13](https://enqlpchobniylwpsjcqc.supabase.co/storage/v1/object/public/imgs/posts/0/img13.png)

The key words to know everything is properly installed are:

```pascal
Successfully compiled
```

and

```freepascal
Successfully executed
```

If your output looks different or displays an **error**, feel free to check the the [common errors](https://waspscripts.com/faq) page or join the discord server and ask around there!

That is it.
You have successfully Setup **Simba**, **SRL** and **WaspLib**.

Now you can either **make your own scripts**, or put other people scripts in your **Scripts folder**.

I also recommend you to use fixed mode in osrs though it's not necessarily required.

**Have fun Botting!**

# TLDR Guide

Download Simba 1400 **32bit** from here:
> https://github.com/Villavu/Simba/releases/download/simba1400-release/Simba-Win32.exe

**IN WINDOWS IT'S VERY IMPORTANT YOU USE THE 32 BIT VERSION**

Make a folder for it, name it Simba and place the .exe inside.

Run it Simba.exe.

Open Simba Package Manager, the rightmost icon that is a box 📦.

Click the plus icon and paste this:
> https://github.com/Torwent/SRL-T
Click Install.

Click the plus icon again and paste this:
> https://github.com/Torwent/WaspLib
Click Install.

**You are done.**

You can now download a script or make your own and use it to bot **Old School RuneScape.**

If you run into any problem, either read the whole guide or check the [faq section](https://waspscripts.com/faq)

Using fixed mode in osrs is recommended.
