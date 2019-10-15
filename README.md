# Week 4 Day 1 Homework

Day 1 Homework

Why use a multithreading environment in android?
	You would use multithreading when your app is performing intensive work such as doing database queries and accessing the network. These task could potentially block the UI Thread and in doing show cause the UI not to be draw which the user could be presented with the dreaded application not responding dialog.

What is a deadlock?
	If your application has two or more threads or apps trying to access the same resources at one time then you end up locking the applications and threads for obtaining said resource.
Explain Runnable interface and Thread class
	The Thread class allows you to create a new thread by extending it other classes or extending the Runnable Interface which is implemented by the thread class which provides the means for classes to be active while not subclassing the Thread class.
What are Executors?
	An Executor is an object that executes Runnable tasks which allows abstraction of details of how the thread would be run or the schedule would work.

What is an ANR and what are the causes of ANR in android?
ANR means Application Not Responding which is caused by blocking the UI thread, or if the UI thread is not the main thread then is block the main thread.

What is StrictMode?
StrictMode is a tool to catch things that a developer might be doing by accident.

When should we use an AsyncTask?
You want to use AsyncTask when perform operations that will push results on to the UI thread.

Explain some problems with AsyncTask and their solutions?
	The AsyncTask push all objects onto a single thread to solve this we only want to push small operations on to an AsyncTask. AsyncTask also can cause implicit-references issues, as well as explicit-references issues but it easy to work around that by creating a WeakReferencse.s



What is a Loader in android?
A Loader performs asynchronous loading of data.

When should we use a Loader?
You use a Loader because fetching data directly in the activity or fragment could block the UI thread and if you fetch the data from another thread you have to mange both that thread and the UI thread.


what are the benefits of a Loader?
	The benefits of Loaders are the ability to run on sperate threads, simplify thread management, persist and cache results, and implements observers to monitor changes in data.

What is a Handler?
The Handler allows you to process Message, a class that contains a description and arbitrary data objects. The Handler has two main uses; One is to schedule message and runnables to be executed, and two to enqueue an action to be perform on a different thread.

What is a Looper?
It use to run message loop for a thread which the interaction is done through the Handler

What is an AsyncTaskLoader?
An abstract Loader that gives AsyncTask for the work.

Briefly explain what a HandlerThread is
A thread the has a looper which be used to create Handlers
