# Accord.NET Framework

[![Build Status](https://travis-ci.org/accord-net/framework.svg?branch=development)](https://travis-ci.org/accord-net/framework)
[![Github All Releases](https://img.shields.io/github/downloads/accord-net/framework/total.svg?maxAge=2592000)]()
[![License](https://img.shields.io/badge/license-LGPL--2.1-blue.svg)](LICENSE)
[![NuGet](https://img.shields.io/nuget/v/Accord.svg?maxAge=2592000)]()
[![NuGet Pre Release](https://img.shields.io/nuget/vpre/Accord.svg?maxAge=2592000)]()
<!--[![GitHub release](https://img.shields.io/github/release/accord-net/framework.svg?maxAge=2592000)]()-->

The Accord.NET project provides machine learning, statistics, artificial intelligence, computer vision and image processing methods to .NET. It can be used on Microsoft Windows, Xamarin, Unity3D, Windows Store applications, Linux or mobile.

After merging with the AForge.NET project, the framework now offers a unified API for learning/training machine learning models that is both easy to use *and* extensible. It is based on the following pattern:

- Choose a [learning algorithm](http://accord-framework.net/docs/html/N_Accord_MachineLearning.htm) that provides a Learn(x, y) or Learn(x) method;
- [Use the Learn(x, y)](http://accord-framework.net/docs/html/M_Accord_MachineLearning_VectorMachines_Learning_SequentialMinimalOptimization_Learn.htm) to create a [machine learning model](http://accord-framework.net/docs/html/T_Accord_MachineLearning_VectorMachines_SupportVectorMachine.htm) learned from the data; 
- Use the model's [Transform](http://accord-framework.net/docs/html/M_Accord_MachineLearning_ClassifierBase_2_Transform.htm), [Decide](http://accord-framework.net/docs/html/M_Accord_MachineLearning_ClassifierBase_2_Decide_1.htm), [Scores](http://accord-framework.net/docs/html/M_Accord_MachineLearning_BinaryScoreClassifierBase_1_Scores_3.htm), [Probabilities](http://accord-framework.net/docs/html/M_Accord_MachineLearning_BinaryLikelihoodClassifierBase_1_Probabilities.htm) or [LogLikelihoods](http://accord-framework.net/docs/html/M_Accord_MachineLearning_VectorMachines_SupportVectorMachine_2_LogLikelihood.htm) methods.

For more information, please see the getting started guide, and check the wiki. *Note: the wiki is being gradually updated/rewritten followed the recent merge/refactoring. Please do not hesitate to edit it if you would like!*


# Installing

To install the framework in your application, please use NuGet. If you are on Visual Studio, right-click on the "References" item in your solution folder, and select "Manage NuGet Packages." Search for Accord.MachineLearning ([or equivalently, Accord.Math, Accord.Statistics or Accord.Imaging depending on your initial goal](https://www.nuget.org/packages?q=accord.net)) and select "Install."

If you would like to install the framework on [Unity3D applications](https://unity3d.com), download the "libsonly" compressed archive from the *framework releases* page. Add the framework binaries contained in the Release/mono to your Plugins folder. Finally, find and add the System.ComponentModel.DataAnnotations assembly from your system as well.

## Sample applications

The framework comes with a wide range of sample applications to help get you started quickly. If you downloaded the framework sources or cloned the repository, open the *Samples.sln* solution file in the Samples folder.


# Building

#### With Visual Studio 2013

Please download and install the following dependencies:

- [T4 Toolbox for Visual Studio 2013](https://visualstudiogallery.msdn.microsoft.com/791817a4-eb9a-4000-9c85-972cc60fd5aa)
- [Sandcastle Help File Builder (with VS2013 extension)](https://github.com/EWSoftware/SHFB/releases)
- [NUnit Test Adapter](https://visualstudiogallery.msdn.microsoft.com/6ab922d0-21c0-4f06-ab5f-4ecd1fe7175d)

Then navigate to the Sources directory, and open the *Accord.NET.sln* solution file.


#### With Visual Studio 2015

Please download and install the following dependencies:

- [VS2013 C++ platform toolset (for compiling some unit tests only)](https://www.microsoft.com/en-us/download/details.aspx?id=44914)
- [T4 Toolbox for Visual Studio 2015](https://visualstudiogallery.msdn.microsoft.com/34b6d489-afbc-4d7b-82c3-dded2b726dbc)
- [Sandcastle Help File Builder (with VS2015 extension)](https://github.com/EWSoftware/SHFB/releases)
- [NUnit Test Adapter](https://visualstudiogallery.msdn.microsoft.com/6ab922d0-21c0-4f06-ab5f-4ecd1fe7175d)

Then navigate to the Sources directory, and open the *Accord.NET.sln* solution file.


#### With Mono (Linux/xbuild)

    # Install Mono
    sudo apt-get install mono-complete monodevelop monodevelop-nunit

    # Clone the repository
    git clone https://github.com/accord-net/framework.git

    # Enter the directory
    cd framework

    # Build the framework solution using Mono
    ./autogen.sh
    make build
    make samples
    make test
    

# Contributing

If you would like to contribute, please do so by helping us update the [project's Wiki pages](https://github.com/accord-net/framework/wiki). While you could also make a donation through PayPal [![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=N4Q6YQSPWN8BG) or Flattr [![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=cesarsouza&url=https://github.com/accord-net/framework&title=Accord.NET&language=&tags=github&category=software), fill-in bug reports and contribute code in the form of pull requests, the most precious donation we could receive would be a bit of your time - [please take some minutes to submit us more documentation examples to our Wiki pages](https://github.com/accord-net/framework/wiki) :wink: 

Join the chat at https://gitter.im/accord-net/framework
