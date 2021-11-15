# Tasks and Back Stack
* task: is a collection of activities that users interact with when performing a certain job.
*  The activities are arranged in a stack.
* The device Home screen is the starting place for most tasks.
* When an activity stops, the system retains the current state of its user interface. 
* Because the activities in the back stack are never rearranged, if your app allows users to start a particular activity from more than one activity, a new instance of that activity is created and pushed onto the stack 
* If the user presses the Back button, the current activity is popped from the stack and destroyed. The previous activity in the stack is resumed.

### Managing Tasks
the principal activity attributes we can use:
* taskAffinity
* launchMode
* allowTaskReparenting
* clearTaskOnLaunch
* alwaysRetainTaskState
* finishOnTaskLaunch



### Save key-value data
 A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them. 

 #### creating a new shared preference file or access an existing one methods:
 1. getSharedPreferences():we  Use this if we need multiple shared preference files identified by name,
 2.  which we specify with the first parameter. we can call this from any Context in our app.
 example: 

 ```
 Context context = getActivity();
SharedPreferences sharedPref = context.getSharedPreferences(
        getString(R.string.preference_file_key), Context.MODE_PRIVATE);
 ```



 2. getPreferences():  Use this from an Activity if you need to use only one shared preference file for the activity.
 
   Because this retrieves a default shared preference file that belongs to the activity
   , you don't need to supply a name.

 example:

```
SharedPreferences sharedPref = getActivity().getPreferences(Context.MODE_PRIVATE);

```










