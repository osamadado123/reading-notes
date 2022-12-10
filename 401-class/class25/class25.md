# A Beginner's Guide to Docker

This is a beginner’s guide to Docker which is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.

With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally. And Docker can be shared among team members so everyone is working on the same setup. Wins all around.

What’s the downside? Complexity. Docker is a complex beast under the hood. However a little knowledge can take you a long way and that’s the goal of this guide!

## Linux Containers

Docker is really just Linux containers which are a type of virtualization.

Virtualization has its roots at the beginning of computer science when large, expensive mainframe computers were the norm. How could multiple programmers use the same single machine? The answer was virtualization and specifically virtual machines which are complete copies of a computer system from the operating system on up.

## Containers vs Virtual Environments

If you are a Python programmer (like me) a common question at this point is, what about virtual environments? How do they differ from containers?

Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

# Library Website

Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework. It always must be added to a project after Django itself has been installed and configured.

In this chapter, we will review the similarities and differences between traditional Django and Django REST Framework. The most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

To illustrate these concepts, we will build out a basic Library website with traditional Django and then extend it into a web API with Django REST Framework.

## Traditional Django

Navigate to the existing code directory on the Desktop and make sure you are not in a current virtual environment. You should not see (.venv) before the shell prompt. If you do, use the command deactivate to leave it. Make a new directory called library, create a new virtual environment, activate it, and install Django.
